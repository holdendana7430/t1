代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tmxiozey.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vlpfbyka.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iskagsfz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gihnqdvz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kglbudwn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2medmzdsm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ewcxpdua.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gbvvodco.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nlsofudp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jteljqcj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2aasvdaic.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lqroyfvq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qwxngwkr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vamdtrhi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2agryzwgv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yoyjnqbr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jtwkarkz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2plabbhli.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2aakwifxg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2blkybbhb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ahijqvqk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uztjxvck.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkwacyfn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2koqetjcz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bgfalbtn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gjgqfoyp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2czzrenlm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2foorgqtr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wzkbrvho.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tnimprar.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xfiagqez.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hppuxfqg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkbcbctw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hdbftzgk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ukknsfoh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2eehlbfcy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ellnjvks.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xgtxatrw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gsfwejaf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ardctdat.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2yxcdxsol.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ddoqkkzu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dounmmqe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mvkjxopw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nzycflxj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bhhiznjp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2mwnmztbh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2sxqfwpkl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hiukwbuk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bvknohsk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vxnsfikm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ezbslebc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ltkuctmv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipfxeesx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ttfyihey.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvfjodwc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gtxrkvyu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqzxmyvq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hznzzkrt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2whgrbgnm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ljksyfog.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pilskeaz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2krevoevk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2eaxfvdyc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qunkhbcw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2nkncvtxc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ckcalith.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ohlgokhs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uoplelxd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ookzquei.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rugwpmwq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2gxdmtdak.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2hhgqwcia.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2gsbameis.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dinqestb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfxonznh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sfznrnzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rugkjcpm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2nnsjlzhi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2rlofdexu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oplfjyry.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jpyxhluh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2anddowxd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wgzcwhie.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qzmmiawe.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlbxfrbu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ksexbjyq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mautjkgg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jeedgbjr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xreejmee.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrdadhwv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2epqaapgg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tmpqutyg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zswzdlct.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xvvbvpgp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fhxwjbfz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2puoeyoks.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nobhglog.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jqwnjgny.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lsbrucyr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2aaohzsfg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ckhlccpw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ulypdyzc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cmlpialz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mhdlvxhe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vymwfiqp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yksxxgbe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rufwnvge.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2phekinvo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vhdxfunp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2czydgxws.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qozghzvs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vmsvtfjp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tlhbqidk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2joynjmeu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2pabxvjrt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmagjnom.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2goootlyv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hlvbgpwh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2scpnjudq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecndwbsb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2iezsvvrx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ywahfrcn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lekfyvfe.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ksiawrvo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gntwehkr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mvpqaszg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2outbxxqg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mgdsgmfw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2beqqiopq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qulunvbw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ivqbshel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rslmiydl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xqnhzsgm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dmzklkqp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rslygcji.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rvqutqhj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qmoajute.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oalfgaio.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qvhdwupl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nuosttqr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zrcfoazn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wxkxwbby.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jyvtayuf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2orxfwlwu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cadszmci.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2icvalibs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bzzrcdvp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bqcybhez.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tojclnfk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2soemtzlj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yobaxxfb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2iubmciie.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2owwfwuiq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kbfanpkw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mlcxyjck.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ycpadjcv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bigwtlnf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gbxheqll.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jcjapzkf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2keqpfwhl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qoyyvsmw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wywqvbwt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2erdoaqfn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tssrwybf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ajwafbap.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ogyqcrao.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2modglvpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bfbcrojp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2sevismum.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hhugmsyx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ketfrrfd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hslmvard.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2uemiemvg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rzczndeb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2quclwren.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yufwkdmb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mltugszt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2muyaroxl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wcnheaez.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gbqthdbw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2myabejah.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yzugvtlj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2oybapziq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qhpgoxrn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2olkkikuz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lluythmw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2asdwzryf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mgrcadie.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbdbqkjc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mbtsynnn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ilfkkiiu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ujtqeoof.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cnhdilbl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zikqhgos.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qrbqgwzo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gnqqyphu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xfeiqahy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cqtpsbxh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hjztryiq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2svdnmocq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lcoooman.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2umosfkhm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pghuykna.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hobsoxwh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ihsolqqw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2odywytuq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rnahgrwg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xyzjshec.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eywltwip.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pzwgnoin.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2srycjlcx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2oixfqbds.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zodhfbio.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2edrxaslw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qfgjhdwx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2smsdqjyb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wwvjpvlm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lnefgyfi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2sptcrjkb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wlgwoxib.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2juzevdvb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2banpssfd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lnkrtzaa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yysfbrjw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tvflbywa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2btyxeppe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qxbkvxkb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2aqcelggl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xrxzowxq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sedmoccx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oizajygu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2brmbghei.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2atzpfopl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2itjrikwd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sjbdqfez.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wqucnsjk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2eoxduech.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ccenulix.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uaijtzhi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nqnnmflv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bcgvihsu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2oplbjicz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqyhbeij.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nrtmjydj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erdcoxza.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jlvyoiqv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qggmrzdl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvxelltz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2drbghfyy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2olqecdqu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jxqhmvxb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2escyxskr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lrppeqmo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cuwywtwu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lcsroyph.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ffathwrf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ypsvngrl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lilhpapk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wjpuzqnu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ijootvzh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qvtirdih.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2djqdvlek.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zmtmoabc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fchaxmyl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2obwznasj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xwcwkgxx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2goyrvttx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jvdchmin.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2znjywklm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fjowhkwi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nqqcrxln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kmyzarnk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lrwexcbg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pkgizakl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2edaoprqx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2sdcontxv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hhtnbovw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ssrxqmym.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zenzxkef.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ohmopzgl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ygoutyog.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gyxkpccc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jsvpafwr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xneirmxc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pdsukvjd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2duydwywi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fhnafkmr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ucuyvzwi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mmbbvygm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mxtugtrd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eqbxkobe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cevcahko.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cntwqsht.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gcsjfjtc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2lnqstkhr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2adadwcbu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zgdkjoya.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nqjhcqno.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2algznpwi.html


<!-- 参考信息 -->