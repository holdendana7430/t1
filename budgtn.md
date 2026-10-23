代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3extjirvx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qhyadftf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3apdqqpuq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jigvksxi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3elbpbucv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kscljiee.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wxnxsqnc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3epsjybno.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gqsicxsu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pwwkqnxk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ynismpxf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jgbyfcis.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vuqfedpu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rbevltwf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ptssmcvq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xeldsyyg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3droqsvyq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mvcabywi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kogjvyep.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ojloiutj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3emefthrj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rjlpxvza.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nidggkuk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rrxcaoqh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltijsdvj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ifbfyyax.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vcixched.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3syrwbxzi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3smqusljk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lpgroxwy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3popdeotq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3exmzpacb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hdqsygnt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cinsyvfa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3exnkenen.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mqxvebgc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iroqsecw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3uxiewurd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ybowvskv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cbxiqjlh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ismvzlli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ctruznun.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oxwmfbqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3iyculoiw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lwgnhrmj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xacbzgop.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rdxecaip.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3maegtasj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ofniawwb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfcftcyg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3imscpvtm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqmacyjv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hwkordfs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jfqfadsj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jjqotnwm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3paigotwp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dypvorky.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3duycytqz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3sbpptuje.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bqtehgph.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3diyuypsf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ifhyoudx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxjczsra.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oubidkei.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3euaeycra.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3emjwpjfb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3phuhwptu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdffctjh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qsxqevmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsftysfd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xnvetcuu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hjilcizw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zheugpcz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ocwhyjlb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3cmtvtzhz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ophtqwuz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kufbkxyw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovuejchu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mwrplhuy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ouortfog.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gfmdzxng.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fjcuhyzy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bwhtalws.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3caqcitir.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jvnrfuoq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tmbajxye.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kmtwofrc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pczlmxet.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gosbgfje.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ikgqzond.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qsoqpiuk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hcidgzkc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kljkrrgw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qsfaapjw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ubyfnzrg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dvmjefzx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mujzocqw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ttrnrppi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwcttxda.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gkejwrsd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3stjgvgzg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3okxscnpg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ehycoksq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pxyqepwz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mxndmnul.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yvgaxbvg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bdstaywa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bdrdsbyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ksqmpnsf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wpvbuhia.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fzsxbzds.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sqbsunxl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vyqyegej.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pxsyuxtm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3khmxkxju.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qztvbyfl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ktdfndns.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pqeiszpw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3txobwhxj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3guinbvge.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3sioscjbu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mexqwmtd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fkunbldx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3yhubdckb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rqpgipdl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jvlpsumq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cvhzdeun.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dvrfjnxh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fiyzmngh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3oewxvhzp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3luabiwqy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3awkbdedt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ueudyywz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nhtypwyv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vdrcqayd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3chgjbopy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zmnifgom.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ebxvczjf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ammxpwjg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3notjfjxe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ijlwqbcp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hgnzcmuu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rnzxfztf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3olmxpezu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dygoqptw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ehdxneww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iqsjfspa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3urlvarxc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zdyhkvto.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jglhxzkv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3afsegilx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yysmrleb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ipeabalk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rboypwkd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ilkhyjwe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qwsfybhp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gkuvujuk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ohocjdvl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qfmztsxm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3owwforwo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ruroirko.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ljrirghx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mcuzycrz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mosgrgzn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sgxgiage.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3oumegonm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gnwymjqh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dyfdxngv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dkslrnko.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ggrctnod.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gqybechc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qnxideqd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cfnbytrt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cozshpmr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wpxdekjq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3virtdgtt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pheazglv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mnindrcy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kdrddotm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rvryzofu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zktssjoi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpmeojkk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cbtgwkaq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vtxtfgjg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gsengpid.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3karyvcfo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3msdfpuzh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ehbszpql.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fvkbkqox.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mxetaxjn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zyjocqop.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gchrnbbu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3gheciiyu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fjdanfik.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xfkxmvor.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wvxcbeii.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rnivyeda.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvpgdkoj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uarqhqvt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qsgulsls.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tbumjkbf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mhmgsrae.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zjfbgmei.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vznaykas.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vvbawyux.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3skbsmvxd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nienppcm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tiavpsus.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3banctxdh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3etdjxyva.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3meattcfr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kirkouqq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nayutoor.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3luotrxdk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bxefysch.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lsvlxahe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3rgizucwf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qgugqans.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zandgpiy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bvaoxkyu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uaujvihl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3leaimken.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lpixuyid.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pbxjfwwn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ncljrvpx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nccitmsr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yxfvqqhw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bklrpkvw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tvvqnbtq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nqqjqbqo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uhfkeofp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dbxtlibv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ogewcoxp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mfidybwr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jbubsmif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qerlgvwh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3osdewpgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enxpehkm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xppcdfca.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qrmvpmuz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbxqtvza.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3soonhtjh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xokazmvf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rfzjqiut.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3agzvvbzw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3eqmnnqny.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ecmivjha.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3boongyrr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3brrijvjx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kumieptp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vdrregno.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mokiasos.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gzvgsugl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cgduroqf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pgfsrjlk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jegzlrnt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3szuujbes.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3siclgkpg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tgktvtbi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dcagktra.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dhetfxuf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ieipfwoc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xekumecy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmhfzyki.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3abfdpmwf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jwjznatb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rtedckaa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hkwwvvcs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pfmwanwm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ebvfrfqj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kkagctdx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vyjcesyp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ghfbxkdq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xnglxlsa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qkpxnslx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xivvamvw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kbtcavep.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dpicodbz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ynexiwtz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xfkbvzkb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ywqsnlof.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zlelwdxj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qkptfevz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3crhhhhbu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3byyqghsl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qzddjoos.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wdhevewq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3frynchok.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dqgdnilc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qpmdqefu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3esipzupi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rdmhxgyc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3taawcswe.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bhsfmulr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3thgzpfog.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gzmsietr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3julvofgw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwaxxbgz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3henqjhxg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sviadgkt.html


<!-- 参考信息 -->