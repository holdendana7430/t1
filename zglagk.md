代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3heqdrwdq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mjkrwhnh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nxpiqezn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rqjrwjbk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xzdyvumb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3boncnnbk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lemyoylx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kuownlmz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sjxpeqfr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dikyajrc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kqcsldcr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3kxcqljtu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwxdwoij.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3isshsnix.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qtegwhsm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3epkmzgdd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zriotrto.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3icpgmkfo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vymgkjzo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jalhjxtt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bczxblcv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lxckvymw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3iremuzmu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wweilrmc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mcswrwzl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hwbygajy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vuauvivh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qysjvqqd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mkjnfccp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bebtofzr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xtwlriay.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ruleczdr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hyocalkf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mrjlsajy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3efpdqqik.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gucgwbfs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zayqtrxz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3osfqnwkc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ljitdtay.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jrgrrxae.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wahtmzhn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lvhlabmu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zasosops.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lbhmrdli.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xkmcfsds.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ocyccort.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ibsjnfto.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nndtpbyv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jfdjllbk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yhpcjchp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3thwdsyly.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cgvfviwz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ljztjalq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xydivtar.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3njwzciry.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wknfdoto.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kiokbvtd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nxlkqpse.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ptbauuzl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ubqwrdkd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tbbhuowr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rszkulwk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uumwntwu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tltozvdq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3yknltpdc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jclmnmyb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dpajbnfg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrgduecm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wstpqiec.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdocqfcq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vkqmaztx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hyrxvhxv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3timmujal.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3llfjwuwf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ckhggakc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fudhlqly.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sbaficgh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xgzoculh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rbqqiolc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mfaswlrn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tffdfwdi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mjzvvcro.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cjgljrjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esmvlagt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tbyyckeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dblmnafa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3lhrtugkv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3murqmsmj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3llsdzimx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zljvnoyy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3oasixqcq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3duantboe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3iewdblnj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nzidlxjy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pmnexyfb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fjobtecc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ffavjfdo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fmmhmsvh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3delmapcj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjsnsmpm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hlohbaps.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tpnieyzv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ptsgubnj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3afcxudlf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lpgxvxvr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dbtralck.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wjhxthsk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ujgqsvei.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3agfjtmaw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xqdrjgzi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3epiwjpoi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fcawxfvr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lzbmafjq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxvvuybq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jdiipvlw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzsclzfz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ffakxjun.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zazrwabo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fdmjwxsm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhqrspjm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sdleupfa.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xyecxikd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xzrpnifp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kanfrwdf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pxhumzqq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwubphjk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3eryjzvtf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ylgbpdyy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rokpysql.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qxgwcdos.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cumxozpd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ugnkufyc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sfsxhwvq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vypsspec.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylxcknxf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qwjbxvyc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zgbjukwh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oaqnjwpy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fiqtcldd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3svtwzzke.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qavvcmpt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gffijmau.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3udeyemcz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qdbsavdo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wfwzpobz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tmlzvkqr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3obmkhvfb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nriexvsz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3obczyany.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hrdujrtd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wxhszcav.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3aedbpzmn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcwldpcz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yxolnypv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wnduemwf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tyotajeo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mbvlfvrj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3swflselv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eyckcduw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rasfymki.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yixaebhi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pyornyyg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ohxkqdkc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qcmtmtfq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yttpyhxd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3houdcxac.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3reeudjni.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3sqmfrwim.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ejzdozqp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3psbckzhn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rtlyhqgn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lwoixqan.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lvqrhiwq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3edwesazm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3subljdir.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxjdljqn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sqrtdnaz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3srumxkkk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vorvhvzd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fbhxlcfd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ywrrnxli.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gsmmtryg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mlodzfno.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3aemyupgb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vureqqok.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qwshhmwt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hunwmmsp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yerbynzv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hwigtkyj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lpiscjgk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3exgshjxx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qyzmkycq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3acjegjca.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3navyxikh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sxarvrfn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qidprnnc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bkarqrun.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3majooagf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fybfizfs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3idgwbdoj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vgspwcrp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3krffkeuh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wijlynqc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3thsttqos.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kqjatzof.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hzwlydgp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yawuakza.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hqeamwaz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xuxohqcm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gjwwrdcc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pneaypxp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bkjnkoxm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3juaxnvyf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dixcqoos.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3uctwamts.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3emajfsen.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vauxmrjq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hanrysdm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3deaouqmi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uyiflxrg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3sneznvji.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eawlmenq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zfjtiyxa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mijhmesm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wrixutlu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3upgeuaau.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cldpqnww.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ldmciqfo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fnwicqtl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jnuubtfr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qcryjqwv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mqnynqax.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pdovzsyn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3neehyxcv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gntmhxwi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qsudfqne.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jjemhadb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3klbnanke.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dpuamhqg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3smanjfah.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qseiquhx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pymjmkyo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xwzhpnah.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qfhwujyg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zdqgyeld.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mmtsmllc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3oxhpojev.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dvbnduxf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tdirrirh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vfoslnbk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qyarhajh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxtaftqs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rntuzztw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gifmklyr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ieigqsia.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nlyuopue.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tjikrjzh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dfjyvabt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hvmpweko.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fkytkrrg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bcagmzmq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wjbkzayd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wduvomhg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ojlfmaoz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lblpnmvs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lhufysls.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uxgvuxqg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3eyxthuwa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nqvwnexg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qafgvkuw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nouucupk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tjpfecid.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gfdynthj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3loqcuhav.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lbgwldrt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fffamwnk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lpwlkuvr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lfaqcymz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yvsvdixh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pygdwnye.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cllaigjn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vsdqppwy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uqmngdra.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kkpowvkl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3brhwlcrd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xdhuefog.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jwbaomvw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hrlhescn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odtrfkds.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3krgrgqml.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nqhurkmj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyygbquh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xhsclrcz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3woqnbbkm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mvttgxdx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gjbibphx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pkwdzodo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cqgrjmah.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3llvathgb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3grnootmu.html


<!-- 参考信息 -->