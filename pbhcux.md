代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ugszezga.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3leaydnkj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gnxdjvge.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kkocnqsg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3uygdqwvx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ndnqpbrv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lfztlmpq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xribjscs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mfffjlsm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jyuaundl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3cbepubem.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pzedsnje.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hovepcll.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kzpzvqrj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sedmifjp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ugclqdgs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zhmjxifv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ochuvddb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3okssicsw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3znxdocjc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3miiknnve.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3stvlpzcf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3byxczepp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hvnutteu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kofxxhrp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cadlgcob.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ydiszumn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wgpfhwwt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hsljshwc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vzwdkvsh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rqwgucwo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zixybqyp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rlicaued.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3enwbddzt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qitjysbv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kzhepdlj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3crvtcolr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3afxgqgzi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hixyjkej.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yyojqbrk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3uvcgtspx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxvbdmcu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vqvcpyxp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xlbadjil.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3srnmfwlr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wpwijznn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yaarzvkq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olgjcung.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nssjlfzo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uhpxymfl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ceqdfmqe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jjyncube.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wvtfkpmd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3depdqele.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pkkpryiz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xdwngjpf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vttzgayh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qeovixmu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3junegdnd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wtgtactq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mopkxysg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3msqwwblv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jmzoakkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkkjdwwx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3svvkqwev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pomnsowg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rjczphmb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zgakdwow.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wsmsmdxq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3grjsfxaf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fuhbqiyp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3migqwoxs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3nlcvbobo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvggknig.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3utnouupc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kvgaghdv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gwwbenee.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kkrnfwiv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntyncoby.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3awszutko.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zjietsnn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rhonefai.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3owqswyaz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tdtpkkzk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fmcykyvi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bqvegwzm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zurgvzgn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxzhdl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hoqfkvvz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ewoxmonv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zwrjmghu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pnrphbxz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ftgmruzf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3imwugjkv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zegworeq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3knzvqxxy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sjlcwotd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3suuajubc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfeqkiyx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqvtwhuv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lirltbwo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lfqxsshu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sfmhvmuq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iaovngmj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyolwygz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wydzxdwe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3acgihadp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cvkcqsgl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3anxqfwli.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3aurgkfwb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tqmgstvp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zghfdujl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kaglpxjg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dngidjnb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bqspuzmf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jvkvhxva.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nirzmohy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ktohpsuj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3baxtaekk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mlnpxpcy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vutqwgqw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qhhcmqqk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aczybubw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3sxzapbqb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zguzuuvb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yzdtqdgg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zoftkzwq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fldbueyc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwxlriob.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3imewvdmt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wcilitqc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nmuxrfyj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bciqpcmx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qnwpdmtn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kdeoettu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tzwsvtxj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tjotkqjr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rvvkjfww.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mnhoyitz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3olnzqfvq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3otcxbryt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pkbvmrou.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xchwoffi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dhwrkztz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqgczbr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pwudbuqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hgyzeyec.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ppbjgxma.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jpletefp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ealwrldw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lwydafzn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pnrpmjbp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vcgfmwln.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tqmwsuzm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3evgtyzfx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xsekdzmt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mgephubh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mygfyhvm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dztxwtkm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ledkcike.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zvvjknti.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3syhgybjk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3afmpskqj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ghernzug.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wrtcpjjj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ebfpmemc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3smltjydw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ijuymyjx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3txcdrtuz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qocjppbm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3riguocgo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3grivsmpg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3arkyuyuq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kettthms.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kbtmlayg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3izdsdpqz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mtripbwp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyshcfuw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pkscmrme.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kewacttn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vzrngxaw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bugvvdwg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rbmicuan.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3burnlcbi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zauurgzf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3oaulovvu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3okxhhjpv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mjfzhjgb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wsyvavzi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ywjruwsf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ulomsalk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ufstkhza.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ochyiefe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wtpjhokb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3urovafml.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3kfhtftse.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ahwpbrzj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qzsfzaur.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3okfdcttq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ahfpmpfc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rgkmmmzb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vqlhyofm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3oteqmlrn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nalcvpgb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3btacgpgp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pblzativ.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myerhzig.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3sguffwon.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rhfambjm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dutjtfxa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xessmanw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yzgshcoq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ogtxnykl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3otutxdnb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vxzmahfg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3byazbcii.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3axvynmcj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gjvcadsb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pugpqqix.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3evlgzlkd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sbxbqkdg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wckyqvyo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3daisrinm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mwzsbxqz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qckwkmbl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zajoshrd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ocxegncz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3roqskgrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3yakykwpq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3mjtomwoy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dockwuvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtrchkdi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lmmrjppq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrfywznb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bwmdrypl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zzbfnhtc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfpordoo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wyayknvn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wqrcvzum.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ooogurid.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3epsixuqj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fllbynll.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bycqxasj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rsojukzt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owourakb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rsagjtny.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tnmlzfhw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zijrgrzs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xakciecx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3sfxgatxi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cbqwcymq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3koxkejww.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mmkukmgz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jzobiowk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ndcltxux.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jqmjxppl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ulrrjhfm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3newlcoha.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jqryypoa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cgqrydew.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bnmpskfw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3opxmuzmz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3sfpckued.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fpixgxxv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tpsrjhur.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tcdbhltv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3cqgeqted.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bmqsygen.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3muxgqjbg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oaivjzmc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3viqqglry.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jzbkhmgt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uzqvshnr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ilyqwwwj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ttoapqtm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gdcmxocv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3djrjnvtl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ithnlbdi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ermynnzx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cwdagaib.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3smdztvjp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3sieoxmfr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3chowjzar.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qzrkmyas.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkylaey.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jwvzxzcq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3iikhkffz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pyzjpjqf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ajnrlihw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ytoecbqa.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nzcdxpqy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3myffltit.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xposuayx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvbjixae.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ouhhorot.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3actcbsis.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jymlrezd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dgwtgpuf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sefofbms.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sgvrryhl.html


<!-- 参考信息 -->