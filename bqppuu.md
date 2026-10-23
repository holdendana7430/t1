代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3haxvjkyz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gblvyzna.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gaqlahnn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wotlruug.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qvwbpuls.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3elbjeedy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3syigfakz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3dzzounde.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gicwpfkw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3codjzhru.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dpvyfdvg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tlsjmnfz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iworacaz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ltnabpgc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bkplikvi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rroalrxf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3seoznvzm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aoeywyml.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3efbpooro.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3muwrimke.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ufbtxyxs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ggvbpppq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3prbsuwrz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kcoqqchj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wsmugbwu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3flcrokwc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bjkcwwta.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gzrbetaw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rfealwaw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lpuefoeo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hkjasosv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cihotbvo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3baziwyou.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ygahpgzf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gfcvdvqy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3midrgqxc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kjpfecyw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yywrkelt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tdpcwlew.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jfowsilj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fccwkcop.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3bejngpuq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3edzjcczl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rimlayem.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3tjrlkqpq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fsaabgkb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oebkwfln.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ovaownxl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pinoofwc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kiiscqrq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3slzomspg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bimmsiqy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3uzhhcxhh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3cvhwsmoy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3irtvzmzq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kvtmcthr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lcsqlaup.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnsbogss.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3haqongjg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbtktsfl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wyiflzrj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3koiyfdmd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wvykrqfo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rklofssh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fgdztsvb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3elukhxys.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gdnkgayo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3eplkevtf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lwhflweu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kyzzjxal.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3somsfpde.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3osvaucmj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fmkmroeg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jcgjqxwp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mffnbbzx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3sbrikrkt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ugixfsbb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rchzrqiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3bcmemuhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joywbded.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3benbmtdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woijcjuj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3eazmokkr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wffdkmyw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ypeompls.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3syicecfn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lbvuehnm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bgxfwvlq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3adlbdigw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yrdvmhih.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tbbudmvn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xzbspjdi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3oduoikzi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wlsdjgfs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3exemujat.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gztloxqo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pnnvvmir.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mtnmnxys.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yfhnjoox.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ycixwbhz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ketrazrr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uhmjoius.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3grkmvzvr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3laroszcr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xthuspnw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3esnsffyx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sunptxlb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vbhtqylh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ufpaeamd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3sapytung.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3adrirmtg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ucdouikt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ktzqkpbq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bkzrkmrd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3aunbmqlh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qhqomyza.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3nqsfiagv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ouocvcgg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3woyprfgt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ykqakulo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3smkbpalj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kmunxvzl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecnemjgw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kbdttucv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3upexickg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ufshioin.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqbvjvae.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yrfovtai.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xkabjosx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tcodnhzm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3auiqcpkv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jyfpoqqu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jtrkdqqr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ecfsqtec.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bflaomez.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jrmvwwud.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vvfmovdc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3apprxcgk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hnkzexnr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3abppfvyz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hzexzfhe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lutreeiq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ntfpoatu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3feuvhjmn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3imgdggag.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nfmzhden.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kbmuygni.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dstotlyj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cnbhapyy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wwxuzvou.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fgnkitbl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qpaumlvz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hpmqgdcy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qkphctjn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mnirnreo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nttukswb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3eytiolxl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3deitmwbs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pvnrutxs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3atonhatx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3epppwfzk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3twkabxzp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3idmgdkjw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jqinnxfe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oavfvkhl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cgftodps.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3tvrnomlr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wrqryzhu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3synhgmda.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3htawvmba.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hcahmwfm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnkoeckr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nrhxofjg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fzquvxsk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3btlkviii.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3sjyulwqb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gnndeuxc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mpvrgaed.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wqkpmopx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nqnlmrvw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ewswcmqx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kshtnvgz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kuqhnejl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3natthbvd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wxdcvgkx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ffdpswie.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gqkvuqnd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3acmvizwm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3czrguvha.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3noohskdd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3pmrqiksa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kuxhtpuj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rdbpuqol.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzhgqmrk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehbeafrk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pxvxymfu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ksybswin.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3niscotuw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qrhsbdtu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tizxgbko.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3svtcimki.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3temempni.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3trhmxisb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3awpirglh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kumgjbkc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cxqljnhh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uryjocpm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gegbukte.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bfibsbgn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xffdndpy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mgnsegdd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3smuqidgc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3iulyohhv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3iewzukrs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3uotllqam.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wntkvqzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3eghyscwm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hvglucnm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3krckeebm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gvrggoln.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yfctualx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dkvbktzw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qdxowrzn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vklesygm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xvcfcgdc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mugpdsak.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dwvubsus.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xfmdxmvq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3loytpmpa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3boqsgtmu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jetqkrqx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ewtkxnyb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zmjeujan.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3suzyvpyh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kjrsyhrh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkqlqicv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3voisvsgr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mpkxmzcq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nnrrabot.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rwxffkhz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xkkzcyme.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ijyzsslj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wymxosxj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jcylsmrq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ovmhiixx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nmhrtico.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yrdcuohj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynqzxjuo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dfnyjhvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3boyhspet.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfomcuzl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wgsaezsp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3urmgdknw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nijjphdp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rvahxotn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hzainoxo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mfyvyfdg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sceobopg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cgxyezsd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bxqnxjoz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pauqngot.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eqerlqan.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3micgqztj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3onlsewtp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3oqlxlldm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iaihxxux.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rvnjjbqv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ovipqyly.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ltuuoofp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wkjehkbc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3idszbrws.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnsbcimn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rzvpiyqm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gyyqjmmw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dmxrlevi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdhjinvx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qxldoavj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iuaipbut.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ghjemdte.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3caqrefbs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fwpvfque.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fippyuru.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mbzwvill.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3txcgcktt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jggamwqj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jgxjivvt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3smygsjjw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jtcoyqhu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3oycsyqkj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3onhnqdls.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wmdeotqh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3adzlngqh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aillxdct.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3aaohabyv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tebymkwn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fmsxwwbn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qmiywlwr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3njniazky.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bqxipgjo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zyvhegzb.html


<!-- 参考信息 -->