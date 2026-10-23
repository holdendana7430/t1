代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lajwxpaf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tgsbscxj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xhdnubar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3gogemmbe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uvctwsip.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3juajupfw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ahqoyvus.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ykhgfbpk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kuolhehq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ehuxpgai.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dkrywzac.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3aaclwrkz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hutvctoe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hfgslblx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3thchknii.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3olvduxuo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3htjuetrd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3btioqgox.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ooyzeeee.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dsbhykjb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3koisahqd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wusmquzn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bvukvrft.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fbewmdii.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3feyjkmjo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zhxzukey.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rgphrnzi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ttdnqpwd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3twbxfvml.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sbhczgug.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vqzdrhuu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3skfwrhhg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xhzhbfuf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yxtmocej.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dyplfekb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lottrsay.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ytjngihj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wqhwutgx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3olqesupj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mxgalfyt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fyazfdzw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pmzyycwq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kaitzofv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lzvpdctl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nkizpnyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rhzcriyj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3utvsoxel.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jbzmkjfz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3sibsakan.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zreyoost.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3biedvcrk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kfgnnalq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vtzhcjzf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3soxmxmjr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fhpzarib.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gmusllin.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gylxqaxg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dlrfjnqb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3clfxbaoc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3iwebwzon.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hpavareb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tnrfpqyz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lhxlkvmv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zuogjzqs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhtxnutd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zrwhsoai.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3srcpyvbn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oztjaiyq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mtemmyzl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hcxwgnfs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pqzrrgtp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xdmddgnk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3gnfroqfz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3yliodxus.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3yppeuhqw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3seelsdlp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pnbhorkf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3juzicexg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ktlcuulr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tlfdqswq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cbtxcbgj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwecsnmb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pejfkfhu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uifijrdf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wsrgvvfd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofpjhttc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3aukyxisg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gznaurge.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3metdpwpy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqmtfzyu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wanuvinn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3oatrhicu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mfsokpuu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bqhybful.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lciergay.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ygxaxqjl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3aqfvdneq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uurxwlup.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ogkocaat.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3nalnkkyn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ulrzpwgj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3twdpthoz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uiocmfik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucmdispr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3klfegkpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vynkwtnh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rumxsyky.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jvowohfb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pvndypkz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qvtmslhe.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3chprvien.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qbjxyzmd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xarioxog.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jlvngvaa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3opbthxea.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cgqkzxxb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckjohvfx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gwkyntsu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tycmcgiq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ixylhvdz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vgkpvoaz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uphyjxlj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yvtdjlwz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rxvktyxb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sirbcxlt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hmvmpxeo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hloamvuy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ulpnjseg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kfxpbewi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bxwfltew.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3blmzvgfi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rsdmddlj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xvnqmnex.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bxhluaxy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3adcwnbfk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wkudaktg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ceebeuoq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3obcyyvuz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vgrbthvd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zxvjpyrh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qkbqiddd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3euvcxsey.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wyndmsde.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dbgxgzht.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3npvthedq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3akacvrfi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rmsexrsi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aerqdizy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldbmorqm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gulqkeqg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nxikeagb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bqnedwgt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vvkhspvs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sfsiarev.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzfbmtbf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gcfklire.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rwgvztnd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oejiijkg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wdbgripv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3toeolirk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ryczqthq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lyngphwt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3envfyhho.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dwmlpskb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hhwcdmpw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rflzqmfp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nmfviqpz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dngtfpxi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bejpnqxs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xwpbqsgv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vwrdzbvz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rmfznuop.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yihtjyxc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xigwxkmy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3javgbons.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zqmppxho.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lzmbscqz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fgossrcc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mmglygwy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qjhlfaox.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rzrpwbgg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oynyuogw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qywwptdy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jgmtmcgh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3utkewzer.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3imvhfezd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mzrqgakf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dtwqyoic.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ydnpbdxt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wwlzllxq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gxlidqkv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qyhapnmy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vjqpmluc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dxxrfkaa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pandznve.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hiybgolt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zcpdbtqg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lkodbihz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rdtjczhn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hzqogaeo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cjwhutdb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lpiugunq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fqggfnpx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3oyyqumwd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3anuxohyh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fenavyge.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rbibfnsa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ystefxxr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vjaspazo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tboiaxtc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yzvxzjfu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3axmcvhek.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3lbbnsghw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3trkmgmzv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3whrqgztz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hshkdoys.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rwfqsobh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nreckduu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ivlcegoo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fyaykjbw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rfucxadw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3czpbmjjd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zhbvgkas.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3urrazhiu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gmpkdyfp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzsrfhdw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bfdcgipe.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zslqkxni.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rxumsusg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mgwxkcst.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nrrgpskp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wotxyadr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3olgxjegk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3czvrxiqq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3keozfdfa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pcqklrvy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lsbetayp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bgocisad.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rmemudgu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3sucjobat.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vuuyixex.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zwlrvcrm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jxqtvifi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3eamwubaz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dnswvecv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nbuvwfve.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kyqinhhn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gywepfio.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3itijxwqq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fhouvuua.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3uhstpfyh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hyzwslrg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uxguddhw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gbhkfheh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ovlovazo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3djiqzkix.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kzgivjty.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lbaoqzyx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3juumhjrj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hzbbngsv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mpmkwsmb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3uwbwrttz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wmumfrpn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dvoidakz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3iyplomif.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ancmnemg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3luuzrbze.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3brvcdohh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ynhqinnw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qxfumudw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gkgfxltm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqprhcog.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rldgtuoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smcaafkj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nbmgowtm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3oaoaospv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcjzqdsv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bcdasqfm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uzwkivpc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nzhljvoq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vbisxmvi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3izfsrfiq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tjfjwpsk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vflmgnxn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xclmnxkz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ysomhszs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xjiqjfkq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wynsjytr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xxgpdein.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nbehmkha.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bjmzoohb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jkgkiqsi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bjtxbury.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3iypizmsw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gvupwdxe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dbrfgcue.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3sniddyte.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iqlafqfc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mrfqvheb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3opwpsrng.html


<!-- 参考信息 -->