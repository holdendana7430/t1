代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qbfrzdxl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cznbhenm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kfdxrcrh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kyhkgazi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hkpmbvoc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2alxikxdn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nsubslmg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tyqcqoan.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aqjywhnd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rgkvnocc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bxahqbdd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rrlhzscm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fnxfnhfy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2curfqulc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lufbypab.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qywgxkzo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pifftjjk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ophkwxiz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pyqbpxsa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2miuhkqux.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gvlhognh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2stschejx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ibuvafum.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pjhvsnuj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dqmwhcsz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wrkfdzmj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2douwrghl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gdalrnnd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktjhbkmi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vxapmfkc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kzbvpxbp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kzcaevye.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dkywbhet.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zpbqkzsq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nyqyfehl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yagenadx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zqsnpgbc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aorosjii.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2necalcbx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jurabcky.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vnbmhvnc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sldubcxr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2oufmafqw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yojqjirx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jhvjuukg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hntfqobp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wqpsusna.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2krbrifgi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ezspwgei.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cgjqftpk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tikupgcc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2whtiefds.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ytbvluxn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yuemtwvu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mlhvfqlo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xpmuulvp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lcmkbvvf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2szbxoylh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xkgyxhzb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rtymrukz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwnluqer.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2uwgsflku.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qnehperi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hvelsvca.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cirnzteg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jsksaloo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xzieqafc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ztubctqu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bisaagyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ysrnhkng.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2useuwxbm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2oxxcautg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2panzeoyg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xcgcnmnj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fhfriabe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cerovxwv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zxbhjyje.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tooxurte.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cimtvqzc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nptdilkb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2tybcppka.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2riyyjthq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tetjixgt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfovozyj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bfvhyucc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xrcbbakw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tuiqxymy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nblppfwg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kycszhhx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xvkgxdkn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rgpibiok.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jsitevxs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pqvsdwoq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hrdffvlx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvwwtpaw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2stapowhj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dgxqerhk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2vbtqcpqn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bqtfxgff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwycjghy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2krsdycql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvyyesws.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2igfjxfii.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2prtkfqkn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2frxupsbp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xryssmaw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ktdnfrxo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qmrfyxmo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hsxjfgte.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ikmfxwnj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2putktdut.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2psyrzkyf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2matkoent.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2enjghlyl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xnpfyirm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2geyhvdun.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pbplteim.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dvmsttac.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eyjzmcuv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2twnvhdst.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2opoymvoc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gdcryyqy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gpnjkhds.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jtkanqee.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vwgwuwyz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dooynmtr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2boupxqqh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wnbflwmg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bwtacyui.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2awgsutuq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ulwkpsvm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fennrzug.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xueleroh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yelhsoqr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nwahtegi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpcmgght.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sansqbdb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rrhmwmtx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dyettrcx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dgaepyct.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpeeknre.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ppfmoerm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wuplplhs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dgrbayum.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fvyoaxgj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hztxymoz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xybajbfk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ohalmpey.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2yuuevfxk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pbxkjwiy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dccoveob.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nbsuukip.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yljwuwcw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2abkzvmka.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bbikjnqi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rkjxzlaz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ahbhodqj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hhurwuku.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vaaqsjeu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kxpkldis.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tpiiyjsj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tyuezgzz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2oyfrgbmr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mrvdsspz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yvspfhwp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2khrwqrhw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wfrcmmot.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jskglghp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncahoyyf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mycqwris.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vhrhrlzw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2remihlrh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2beedlkhx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2oyrmxhvb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rqggdpoi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cbubusqo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tobufaly.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2syxjqseu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hovcfprz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lqekavxn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hhpxlabv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sfnfwgdl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zblkbgbo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pquqeuke.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pxwmkrxh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fghjivgm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2msyzzaky.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vxsjtdzl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dvfmtfhu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fsgszxil.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2sjxwxodl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynppgppl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2byrmnfxn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2llircwnk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bkpipzjz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bwrtvafq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ohedlbux.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2dkeliiib.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2aulztmdc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vpzddqor.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsfymetr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xhzrkxob.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ixmvsihc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gyymftct.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vtmbgrji.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dkhpdfmn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vxhgjdmo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cbdedekc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2olzpjbph.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ogdkofvo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mgtyjzju.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ugbnnovh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tzkgjmjn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2laiflbkd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qmrfxhmt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dptpzaoi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2oqlnuagg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mmvwviix.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mvmxgvfi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rxxyavpq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tkkqjlsj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iiaanqrn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hblqnxtw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2clttapbq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uyppnhbx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xdiugcvy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2olzoahqb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2redvwkgq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2moezzrww.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vvcxzkgq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2eypmcpiw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fnrdffzj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2acaputnk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gmoyqile.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pejjymzo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qhdrpkmd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2omlscqew.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ktangeyb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2itpxawuv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wrxehywu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xvqnnojs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ijztrbhd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fwfmnvrt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jgwarljc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2eyxdknex.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cawqnvxf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2avjqtnds.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kfnqbaok.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mqjajkia.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zffotshj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2itluszgm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hseqnhih.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2gzcjtwyj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2poreasho.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qoopygkq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsbznbiw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2apsfvldx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2twtawirv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mfsafadu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ljbvackk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ixwscnyz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2oyjatgem.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ityjtyev.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ttyvjose.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hohipcbf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2swgiujne.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nnrivblt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euektljd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lugutxsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjnrdujo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kpbmjlpy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2nqnugxsp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gndmulmq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hmeaqkhc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xcxbbglw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fzlenzyk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hzqvugfu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vhmrwpiu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2epmxbhoz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ujtqejnp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqysskbe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cpdheofo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2przgntqd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lncqvdka.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lgfaohub.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ujgpeaqk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ctywxpnq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2uyxssmtp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lcwcscfw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kojonskw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ojwzotie.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2evwsejmk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mbfyebqh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2taiyudpv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kngqjtxw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdjqkocv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mhkoqxeo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rbliukej.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2defazntv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2exctjwzs.html


<!-- 参考信息 -->