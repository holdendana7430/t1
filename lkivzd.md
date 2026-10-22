代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dkfgvfyw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2eqbmdrcr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sxeaofkh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kemyvgmv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xzppdftf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2siwwglmz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2onmbegki.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lxhuegrd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ixzukavy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yutwyazm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hpofcxbf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2akrnoaug.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lwhadvxv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jbafwwcf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bqkmzycy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gorasuyd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jykazjac.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bshmeqiz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dxebybxa.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2cojmfxec.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rmhirggr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mekeojps.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2acojjfbv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2prsuzyfn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vrfihvoj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mnfhmaay.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ztkjzwis.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2znabuohx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zefpaanj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rfzstlga.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dlewnmgp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fbokwzas.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oftddtfu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fyspotdl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kkkrutev.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2exkgpxib.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axgwndmv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2knvprnpw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cahfyxvg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2sugbvhve.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gwnuyokn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kilkefrz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wlnsfzhp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bzpruwqh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qhsehvzz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qwozxeyh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ugrdkbcr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bcxoplxu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wwkzzjhw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kpeyfzxy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2eoeehzde.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qxijgrgx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cunolvxd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2akwppjsq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hunbatyu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2sslngufd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ihbqlitb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ctvqmepo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2iwoecqxt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dazyiclv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mktzmmno.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mvymgfht.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2horwlfgv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fxlzenha.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nulzuvla.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hgapsicp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2coxgeiec.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wohgzbby.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xmgjgqrj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vxiqcrai.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nmhtrhbo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rcwathdl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pttweprw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lfqpidwc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtbrkojb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lqhvbcqt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hohgzldv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kdrxizuf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rmsxkgfp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2imjsisnd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wunzatuk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ycdgzlkw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jrdbudud.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jfgmqasi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ltiwctmu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iziikcsp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hggojtai.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfhvehmq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lwflapuu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2osrwluwv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wqbidtaw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfzpubeo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bkhkrcnx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxlinidi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vwrycsho.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xsdcocoy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bdpnvfwf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2upldrbcn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bxmnwcyb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ejpfooql.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rzaruzkx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pximtmyt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bthnnfnc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mmveiqff.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uppfonsj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zhqtxenf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jeugmmdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbyathho.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tjqdjtel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tczijhky.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zwnynwhj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nxykaxls.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zokcneiu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jviggngj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2evyinxnu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2otogjuxk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wgujsnhn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ildeoiqn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uajtugfi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2epslktwd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fhzfdavq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gjbavodj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ltdbdept.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzthulib.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mjjltwgx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jekeqduc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hvaxmuhr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sfrwmegk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rnrizbyd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rokhcfrb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iuemapdg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ibtiozhn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hpxbszji.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2snkkafbd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2evmpzbzx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2krrxdseq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2eheibhvp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cihbjiwr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2opjdlktb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jkmmtygi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vevwhswq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xdjxyjhu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2diormims.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucquvetk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uakfaffi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2djngmgtk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oagutvyd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ofjafhso.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2awcpkquy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bhngfglo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pixlcrdi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jzcjxagg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bygirtwt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nooavjxj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yfblrdsa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2siyrdige.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kmhpjkuh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fmyetcxx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2crkuqvtj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gvdppchi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cauyqbfp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hzukjtos.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tcccfaet.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2utoqxkib.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2beuvkcrr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wrywohix.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ugyzjcat.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cmwcdulz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rziwjgpn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vjftfrhi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jluorbur.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rfqpsvoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qvzscaaa.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qvnzavsy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lcefiptx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2plklmfvs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hevhocvj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2flbqqujk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sgiiiqjj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jcjxvzoi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hivuijsj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vrwjkuvi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2extblqvj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kmpyrsdc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tjiklkcr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zeoixnnf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2utcdawwf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hditjhxm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tpjgzgpv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2widbmrgr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lrghbqji.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xhopmgmq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2asxemvds.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iboakltt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nbzexili.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2naqlsfhv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2brhqycso.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bkwhqozq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2frillmtp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wefqwiob.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hnhggtel.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qfzuhfqj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hwbozfuo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2frwowbdw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2aaphaevl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hdzwwmsv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nhnyeqvh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2elzbptvb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpshbkyc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wxskscxg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hupveaol.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xboobcwm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dkwvjotc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ntlyinfs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rhvzldyc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gnbzwjsl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mrfzcids.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fmeaybeo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dhmtlmih.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zqucshyo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hpapfsxk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhcmbgub.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2orgdtwxv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bljiwtro.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2otwgtlid.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fixvcovd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rfawusuc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2clmszzev.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fucnduwi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2naukzigf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hkzpbgbx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kiciqgxj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2olinttbx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jkhihvdf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2bwybawfi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cceuwjkx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fntxboiq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbglqtse.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gsgzboku.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qcvagkel.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mpwcqeie.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hmklnyhz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pehvyrcs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2seesiqne.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nmyjhuen.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2agkiyctm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xihxbmxg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pduymwcr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jbhppaky.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2iyeufbsq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rmgtatxi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2colzphif.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tkgcxnyy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2falxavce.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tdlhutrc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zecebgui.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wtevzlvf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ndovllkm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2orkopdry.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qudldijq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2duxuzqkt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kaippwoi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2djslktfq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xrsgyehk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fvzsuyil.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2athjjnix.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xhaqkygq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kcljbool.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2upmhuqyg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2plsrihmt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2upoecyzp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ajdpqsoj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2shhwvltp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2abadilnx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tzvfpfug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yebwpmdn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ghtrvpyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rubkfkif.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ydgymhpe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mbcbmbwj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2waxzrlpn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hplwepyo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2lfichxyh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xjlbywkf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2laudiqoa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qgqlhtru.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cytluvcl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jaupulqg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vgopzntw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nvqmqnra.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nkibqqzm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pacrsgbc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gvqdimub.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dzuxojod.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yjufuhpd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2osmhnlya.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2estuzpsb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2slzoeyvq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dokohcfd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2addeaszj.html


<!-- 参考信息 -->