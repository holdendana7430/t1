代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3atlsisdn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3eirggcxi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tzhvxcnf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3alexvbnz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zmkqzavz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3yzfhhctz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ntfyufct.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ystnadiv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3uthhrmlj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3molbmevf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rfhtxtje.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jfdjktec.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qgjswfxe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3snsugnjk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tudyrggf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lourcuwc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ysdxrtpx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dgrvklaw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jnguvvxx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jdxfbrvu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3azgpqcli.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3juseibbp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fhewcoqu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zgyqbxcx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mekjamdz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cgioyrkf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3inunzale.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mqrjnqvy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fzdyiste.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3towwkfcn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lrbykzej.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hgfbamxs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwiijerm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3msauwvdo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3golthwpp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rckinrie.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lmkzhptn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dyjpwgzx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jgcjkioq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aqxrjskb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zklnknna.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzfefzfp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ygdmzyky.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uwbkxpew.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zawwhgpr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zsgrrgqj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3knsyzjev.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hbtlxyii.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tuypzjlx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3diqaekhb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3skuulbus.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ejkbowdt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tbmfigev.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vqdwtbqu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3iibzsbbk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3spvqcmvx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3mfylgixr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zejncnhc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3awafznmm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xjdclpfh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cpnpvooq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ieourlnp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3txlhwbxz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gjqwllhx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnrsdscl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rkewpmqi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3txlbqiax.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jcqkmtxu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3axqmedfx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sarkrwia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jlcztftf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vdvbktvc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bqercltt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3guwezdmh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3brjiygzg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wcmjadfo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3objzucpe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uktyritc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vjerieqw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lqlbjrrw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rumlwraz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdcrxxec.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jktuyxuo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzwebqyb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3smwcgrpy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3preyfccn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sihrqgxb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgccap.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rscyockp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aymdfjdc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3uwhanehr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ezibfajr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rmjeifwb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jbsxhqmm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3adxjxbsu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uqqtjhvl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zuyvpyyh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3eiygcpjn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ltpfomoq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ybgotdld.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ylskonzb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dbteznph.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tyytcaof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqlfbwyf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lfjgtuie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3euljubrv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jlfkfnul.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mnzntink.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qiueoqft.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tsnwprmy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zocvyqwd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mziysnci.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hwskndeg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xpkvnjst.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3elfgaryy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mxiejvfk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3acarousq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ciahisdc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tifmehim.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jgwgaadj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nwuowbsr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zpxgxjpy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uttxrnxq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsnbqyqt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ogbioean.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xyzimmtb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rlazexwe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xsucicnr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vuomxpwo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dnqzyedm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3arnkrgqx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ivbgywnh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3txsmhxdi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ttprbtqv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gesshqdg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kjlrxbbm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ixulvsil.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ucvnbtbo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rblvnkux.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrokqcki.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fivjpitu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3oqtpefus.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3udfvujwy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kxcappmd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvladgkf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xrtraykv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqzchjsi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dkthcjoy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ljmieqon.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rqqgepek.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uftrijlx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mfipxdxu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3keazkmlb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lhhhsfqo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ooaxdbao.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kkyweoca.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lcflczvz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dioqsdtz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ymngzytu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dldwzdrd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3heriogre.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3impgrpis.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dadggrng.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3inpmbtkc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pbfvutgr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3yozqtbeo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tpwfnjhq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uybxbauf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3burzypft.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wxnedmrb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ftddmxqo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3irvtklre.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmmarlbe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zfhjzejs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xczezdse.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3gwyrrjdi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rgmtuxlh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mvldcrcx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3drapbcap.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tqyylnkz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3djupjkur.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yazosmuc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bbebnupr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ufbymdou.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymrtmkpq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jskeduqk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vzodcarq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3csjulgfx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wlumqdkd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gcofekfd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mfbqildb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vukijjxk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3moljmpxg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hglogqrf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3boraoibo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yzhqojzh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tyctcdrj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ydmdnldd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qxnflntz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uajwbdsj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3phlkveic.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ofpxsaaw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tksxzgcm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rpowyrij.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qzqeivgt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3txffjytt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3venytmil.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gqbsaizm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xqrizpta.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kxirtiol.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hdjsopti.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ctguniqk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rhjnnbid.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3amxpnvxp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kmoaiifw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3efgzmtcw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rtzyggnx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qekcrrtm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mnwgjcjp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vgragvei.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wfhpwuvx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qahcebjr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hpmwwydk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fuvuksft.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xmeallks.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tqkqqxrk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rokvuyeg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lsrsgqbb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vefeflqn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hvimejzs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xntxjuio.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3spoupcil.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3prswamee.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yemolkuu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hafekxtb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3aymahxmk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dmxcgdlk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xtstkzxs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wnaxzqck.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3sqjwbfps.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zepxrewm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rqfuqmws.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cxldfjgs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wiwuftmc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xnkadhdd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ujaoimhj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vesqsszu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ootmxrje.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3crznootb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nzlgejgm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3twhjavii.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zmothggw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wczwewda.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3bmytxhgt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3twkjjovm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vxxjedgg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cogittyg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pplpybus.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ohfjcoud.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nwhztpaw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3caiuzhvf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vimhvsmo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uzrqvbxk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mzuvydvm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vrthtlzf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vhzvmfbr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mlxzwqpz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tmkocxcu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ljvitaoy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ixrajdys.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3khseyvhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcrmrhbt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ecwgncos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybqnewjj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3phezfkvx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3conhbbyy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3fywpnkjs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lyrnwygp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bxnqqhab.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3albqipjx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rjatzhqf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3swooeulp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kjaylhzg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3icrekgyb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3stzywoxh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tssthctj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zrcbfwvz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mbemygqm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3emulnpik.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3niolfuyj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3czyhvxwd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ptbksufi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tkwwtvgo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hmkclxps.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kqdsmmtz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oznhqbbm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ukvovujp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bhuhbsbd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tzwhibee.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nkzefsgb.html


<!-- 参考信息 -->