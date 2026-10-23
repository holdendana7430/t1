代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipzgkjhn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3stmlvvni.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zpsbxbnw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3uybcwczy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qvbqpnik.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rleneury.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yxvgmhsj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jbeepkth.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mfyncwof.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vjbdpypa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fmxsffve.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3oskehcfp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ubxqteah.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ndzfyzte.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qzjunwsj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qfmnpoar.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dhgaguze.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3diiihnqm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zmqhyabo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ykxknktw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mxrlozez.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3tbnvevsf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dcamrbtb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3cgdbqiqt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kombwtql.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zrdzmyye.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3djsusltb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3suthejnl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3oqrefoev.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zvgwkntt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ddhxweny.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3klbbprgq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzlrwjkl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hfzrfxqp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3syhckyxe.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ksfdbqrm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3tsumainz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3npkmkxze.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gufyerkn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zglghfsl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qrllxxcn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ketpzvvy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bvddclxm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3blkgutuz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qnodjdis.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vbkrhyyv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3aposiltn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xmicjqln.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hoponoyq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3epmuidzb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mbolvnxy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tutskcga.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nmkefvqs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyhtapwx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wazcnban.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3duqpxurs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dfqftduo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3szqfgobg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3obksmltw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ideiimwv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uwtkgyjj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3eouxqzhf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xciiarqz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3slxydplv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jrksgpsa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qnoybevi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abtdtmqa.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3isshebfv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3awztzrwa.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cywlcvef.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3iqxdfits.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsuiawwt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jzortmhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdvzdbfj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hupqjzds.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3muvrdfmh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vnoyumje.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vqmsnzxz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rrqkcujg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qzieerwg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wtfqwamc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkwhafqr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lsxjdjmv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3utnjkyxr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3osjtnwdf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3phigsirr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3semiuwao.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzsgaxmk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cfaoudcu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pgbuyeob.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dlnsnyxt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qtnxeluw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3uxqqxypb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ueoyzbjm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lvpyxpsp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3aeblubfc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3shbcahwf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oirsmvkj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3opgaseor.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wrgmipho.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nujietqk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kmvoddlm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gzsnrvoo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wxchesyz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ywgellfu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qmawhhtq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cmqngpom.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kxrvoehn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ntcmxima.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ehpxhiws.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ossdltyf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hhvoulvf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pxpodbwu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hznnavfy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wltgpgux.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3txnsysbq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkiqohom.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gldblorv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cpqgamdd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pwbdfcgw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3brmtdmry.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tvfamghz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kwiysgct.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pgmcimlp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3obyqjxgd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uawrrilk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ntaptdme.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jmrjdlmp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3sywepdnz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3psrljjte.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3sqboyiaj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vhenwnht.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3idtbrboy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rgayvjjz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mkflyfmj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hraylrso.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vemzfycm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qzmmjpef.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qplcmpuf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zauxzeia.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wedbijdt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qwtqkqvo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovfecdcd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cbuhfydy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mlgvliej.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tucjituu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cuqfspjt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sffqppju.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nmvqxijs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dpabojbh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gtdbdmbm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mujlzmpq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgrubide.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kqbemmnh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bouockjd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3izssecxj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3chtxhkha.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3idgjetrb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zvbpgyrg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sswpbymg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kjcgrkqf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hjmzoacy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mvtqiiyx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qdbvyzuj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ernjhsyd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lkockiiq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ngqszlwa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zsamuuij.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xphxuthj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fpgtlspm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3slmqeclo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dokdidzn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3grmridfn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hifddfvn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rzkdiljk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dsjbxrva.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3uaslmjag.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nkdajxtz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zewsegmi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3felrvibu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yrhfgung.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3elnpmsra.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hinyjnbd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3oezwznxm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rslaaxhc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mqismcaa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ugkqoghl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pldwhpqx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pouruuij.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hvzctstj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3saifjdqp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ysulvnpl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yqlllrtx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zgdayjtd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bpadizfq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pfuezsrl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nupojvak.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3waxmjsmx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xcixzrla.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bormgelf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3esozayrb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ijxlgdoo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tayntjdm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pmjsjwdg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3glybqkbc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vzmnwudc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3pajcjnfm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mkkxjtkt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sgqyisnm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dmehemdb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3eqzznrmg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3busgmfiz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3smostayq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ccfnzbjg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mjvsvety.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zjjvuxoe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3voimgfac.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hxuvisrl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3idlpmnep.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zbifyyeq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3anmyxkyf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3sfzxpzea.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3roozagwh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ugompaog.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hhskggoy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3psemmjqw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ihxznvgo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yrdznjnm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xuhvtkwm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgnaekyq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cgqkjyqx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3eoghqyrh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3txkrzeup.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3morazitx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3hliyurzl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3etfwwxzq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uwmngbzf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zjopuhqr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yrqrcndj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpacagyg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ujahmrli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smumgehu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jxldksji.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vftytasu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ocahnupf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3udujwvqb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3grdtaqvt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hdesaqlx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vtxdigub.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lvogydwx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3smehtypf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3prbnxdzy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3astfkjep.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hfwbumws.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rzkssezz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sqyoqvdu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3isnwurop.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hvoriuwn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pnkawwnk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3aictoadl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3albdhxgp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hjentrnz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3akgpinvt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jshtahlg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3twlhhhsf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3oonrmvyd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jzlztuxl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dyvqnuuo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dellpekw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dbxdwodh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kngcysxo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mcbdsvtt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qczpzrhy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lxksraso.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3szfyycwr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hdjltvtn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3exbcemod.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewiuesmh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wrdgzryo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3knfmtnml.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kdsoousv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vuousebg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3goadxgwu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3klmssjnu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jogbsosp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qxhvcfzp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ojxaxbzx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3sxhstqxd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hyzqokkx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rbbwwvbs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rtvtnkiw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vshdlurc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3eglhspix.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xdoslcts.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zdtgcogr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rpndfyey.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sgiftcns.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tncaimeu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sddsrnva.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cezphitf.html


<!-- 参考信息 -->