代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jvxepdyz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ibtvmanw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rdwwraac.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nurjnxup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cpdhiqdn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3iiimaqzx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cbcnryyt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hahupeec.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ihfyueuv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wxfjdvbx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lfgfxoef.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbnovvju.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xqwxjihl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gignpssb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ulptnogh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mbhvisrh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jpyqxnww.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mzyqijzi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lrcuctda.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xijovbwr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fsrdlqzz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tobqsfum.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ybrewlre.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3elvkdfgd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3opbfzgwy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jyrbbllx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wfakcfvb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3slmrffes.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wlaiolsf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3immjbahd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3brlpjlvk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rzugmrqw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ludopccv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xmctexyi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rjcrtovr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3igqluccs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdhhlohl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kcqolsuy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3auwcgeso.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rsmfscap.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nejqdsps.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lukiyoif.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3afoipmts.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zwlrtaqt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qkccxcak.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pjrtyipl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3uegmabvf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qbmlxxia.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uvzrrawi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3uqxbbfvp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3drtshxjc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vdqxtmjx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3krpfqiie.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wyjbwzzy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3aathhyiv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mekywdrh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hubtfsxm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ciyzremh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rabcdset.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nchbrdqk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3atbmuezb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqtlhsaf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hdjjuvhl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3yzdhekcs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kmylwkte.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zfolfxnc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dbaffzsb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3oilfjxau.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uuivbeml.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lkmxwgco.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rpidaxsy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibjblguo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pueyetnf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mmjbdsgq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qtjvuuxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iahawxwo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3unjrctxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsfdrxbr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nrsbziyu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3faihhawd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jwbcrgnj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xmhcsuap.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3obmenhod.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sedpvqky.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uzercknn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xqwnjgea.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qjllndwj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zoqlxicr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3amdwtbim.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iewrmwwm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ejevxoat.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lcidqcel.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jfwlgxws.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3feyhllng.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vxnylvvt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gtvinueg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fkafxilq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mxlxdnlp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nprlkogw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3eozvfwyh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qgtwwbqb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ddmcftkq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3aonoyogw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cdrmwahk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3fhwzenxi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxdgaxnt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ulkdcqrl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jbvudqjd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wcccpuuh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mnctutuh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3leghmfpi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqjrngih.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eisrssee.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3atuulqpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3njkyavbl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3eollkcpz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mgxyzoth.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pflhlquj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lddiitjs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qvyaspoh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxfcitux.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rqvjrdlg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rgdqdyur.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3clhiytmi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rdemuglg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vwjghlsr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bprbsrrr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bgiupfxy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zpzowusd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jzwjdfif.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3huchdtvy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hslokzja.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgiyembl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vqiicfob.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lgdgbbrn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jqdqypzb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hqbidmfd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ykukpicf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ebgrfqzq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mgqtojah.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qdokdjxx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qaamslch.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ubygvozf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vpqkckox.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3btdheeoi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ywpaiepx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cisttytr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3yhtsdxxw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jfnxtqbe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xevdgchl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vmwmoxns.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bohzeozq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3heywnkjk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3htdblhsf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3swtewoji.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3joilkwfc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fndgjbjv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rbuqejbt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jhbgdrka.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xwiwnkmk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3suxhcjyw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vakoujpq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fkspeevm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ohlhcesb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vdjecoub.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bktryvhp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lhirtdmh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ezsjhhpf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ksmoubsr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jyjdxmpx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kojkmxvb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hiiauxtg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sunwwonl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nopurvsp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3oumkxodr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cnfunxuz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qjdubqbw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nyjppulg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dhvipksh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3flaugvup.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3obzoxylo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3sekyohor.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ombqottg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3osjhkgbv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3sovcdnoq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3udrtuuqg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3walguxkf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cqqivzts.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3igoqofjw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bnaotpax.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dwpolnrc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zimoiwon.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lvpqpjek.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3snljrtss.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ixfiteru.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bzyawwvd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ncddkurn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vpebcrfe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3awupftnf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ylpjacvm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xubhritq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xdpvxzxc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zphyxkti.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ztwaynjk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3otzposff.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mufcwhju.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gpvpoaif.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ymjertjb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hgrclnat.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pqyyntnr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tapbalpd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vntospnt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3abyxkpzx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kftubviu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3iqozfzwn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3aywmuald.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jjbcamuq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gsizuoxr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qkykeqhv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jkjgajqd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tbuljisn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qqxmdkot.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zwnlwhbp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rhyzhjab.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3iofvloup.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vjiktiuo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nwaedzye.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nftvupmk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ihujpsch.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3faitrhgp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cmbhbmom.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mtgnfxfu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vlexbgcf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bxhsddiy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gffnqytq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cjjmgjtp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ntlbpoki.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3oewlrmwg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nbbzuxik.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bwunygkh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bmcshudx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3foeckyvh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jkwwhzku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aacepnzu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mvcrqwdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihzfwjqx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3daerkwgu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3srsrgfys.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ljmeajxe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ttwmuaib.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wgbpplqj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vtjcjzgp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cmnvqfpj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kkvkwcll.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ithdsnkr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fqavlftq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uoroeloe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmyytghq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3clqqpuxr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sbkjblrj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3oukkxfai.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dgpbctib.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sjqsucpd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dggxigmi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rjifmaoq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3parxhhjm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dnmejsxc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uymxfkof.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xrfbfths.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3eeykdzwk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yhvlejap.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tnevbrrt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ncjzlpri.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xlavkvbu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eemhqcha.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vrpxedrq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3nwywonlh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3exddjuni.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3sczlbwuu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zflqambx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fwoysxdx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ahtqjrzd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ztoonhwo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zhqkobgq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ksjipwzk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3eekyvpsq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3plllwzoi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oehcufol.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dsewyxnl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bmozauyh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nmpsaocg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hqtndrxm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nbbbdloo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cgbvnmrr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uqvvsvml.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3oeuucodn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jhnvpfyc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dtnpdjkq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ajsbngkf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gxtlbcoe.html


<!-- 参考信息 -->