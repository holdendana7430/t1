代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3aklwcmop.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jwtzybzo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wcoqjjuu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3eqpnjpop.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zzvlulhp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oixveyal.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zufdygpe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3dagnmxsk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yprvrdbm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mqiboakj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ynasmice.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3apwqqlyg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jqlmsgiw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aevtztzv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lfnfkizb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zdckzmmj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tufijcvp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lehwters.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3whrayaur.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ktmoeurn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vssoimpz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pzehujfm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3inoeqvhf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hejcpkjg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kerydwru.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zehshiha.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qivdvugj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ocienscu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3znaskpwc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3oxtkfdpz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tggdcdwp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3gchgslcz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3otofzjti.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dtuvoekb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3psdlyura.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3faibedij.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3riwzcqrw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yzpkjmnj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3iojruuqt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3clyrvnij.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3igidwjzk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zfaxxqab.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pqoblgss.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jqrptssw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3drgvptej.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ymtfrrjs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uzxzttvy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3owbufypb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3yuocecqs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vvaeiwro.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ulzhnuet.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3yznzghkq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zfoczzwb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qootsscw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xutcabjb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjrhmfqr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kmdobvea.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggzialjv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yygoedqh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tgsnrufb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vjiwipzf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ydfvqfbg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qisfreph.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tilvlrvo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xszgpctf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dtkgeama.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3gjcjnvyn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mjpwnrpt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dvvrceni.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gvnqzmzl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxwmsuhe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yznfawwy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lmcwruqd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fjquuewy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zjzszcyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kaosssat.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fcategbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhaerncv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nwonvdpi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qhgrrgyi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ydjgscaa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hqqenaxo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ycsfckig.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3eakskvxk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gwqrmvwu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gtrdpfnm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ovbameto.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ldbymdwv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jnnsplrx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kzfyrcgi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ffvktdcz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqiutipa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xzrvvxnb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mdqhkpdt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nwllmmip.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mypbygtu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3deqtnuhe.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vnhkwupq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3sdjxcudg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ulqqbttw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yvqwxkxu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bkodosmi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3arzywqbq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dykvgfre.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pcmosvxa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ywtzqirr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bbhzwjpi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jhfvjugj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwtbzadx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kuzjryqj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iuoanxrk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgrapumg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yluohpee.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3msqdtmlf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3njcjremu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qfabfkne.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hrsxldfj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ktcmflbq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fwllklwi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3htxypoav.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sdzacaho.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mghydsoz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3skqlkloy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zppwjcbh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3epzapblp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fuqprxmf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tedyinis.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zpqtqqvz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bbuopdxf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iwqgusah.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aflzmqgt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zvyjkdon.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ghizrszo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cgegmowd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3yikbyfjj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3pnquijxb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dpwhfcjn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ajuvtwar.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3olwdmmdx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aezslgeb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3crzqsgtt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xytnzdjx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hqpycxaf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vtnohwhm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fjyuucwa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dygstepr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzalafdy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3upqnuybk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rdbutfaw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3otjamrlh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zunqpsxr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ufgleusf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3msighbqj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3syjzlwck.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pbympjza.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3eccbogqm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wqzjiswt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ekeboxcy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3oadrgoxs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qywshkjy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iywttott.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nxiyupxw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yrqbybiy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3uylnvnhd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jydkgowj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nlkohvjr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3klymrfie.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsylffdg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yjkhgtuf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zieszctf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vavxwaco.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3swbjnhdk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dxylqhjt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bfqspife.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3buzxjvou.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vpblzxou.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ptysakml.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yaxfocrz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nufcruhb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ixijdjts.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wjncntkt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ooqiipza.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jfgliqey.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3mjolzhoj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3eesxaifg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wukngtem.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eecvpwfv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mapleglv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lntpkixc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzqdxxuu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3frybbmhp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mhtepaql.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cvgxywhx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3msrwbdjl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qhfgjrfe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ygzkynsv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rlgilfnc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fshfgusv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jozzhzqu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jmuijysv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yykwdzlg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fqsewffc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ikmpzscz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qgumuiuz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3sewyemqc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dgfyvmna.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bjqnpntg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wvprtoia.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ihdljfve.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3toftslhu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wscfzwej.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wosryqzm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pnphyear.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kevinqpb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3lxkkossi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ugaipyap.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3uqkouqev.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fjfmlcmz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dhuaodsc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3buvxupty.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3iordiffz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rtpilwjg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bqytfcaz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iruwjvvt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qcxhalzl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mbkyytxr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hesiyone.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dknwvmqd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xyojzxte.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rhxklelr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3irdmzyjr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oeyfgqgp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3azolwpml.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ocdbqxjn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kopgpeai.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wqdanowt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jberdgko.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mdgywbpt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3tbujlgyf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yllkginr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zccujtmd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3mvniyszh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xqbcfuud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngwmxthw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3todbyaxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apysydaf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3icvefkfq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ficldbbn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tqakkhwu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3seimmvfn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3njvlhyzv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ebldyjnu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pqcbuymi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3whesfqmh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xznnbemf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sxenafmd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3spwcxprd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uwauuqqc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nmdwvgys.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ujkgypau.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lhblsihr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xiepnmxw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fahbftdy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lbfjxwdh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cpuqmunc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rvbtidjq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rpkqqodn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uskeotew.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xjorrkro.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oyphrexy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fyzthsvf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3cpltnnjl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vrbizljt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kxvjnrqn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jiemwfzp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jzsdtgqs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3saqhuueu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3flpapxwv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wdsfrqvm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cnnacypz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nhqpghcg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3snwybbek.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jffixzdc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ghegyhzf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hvafjgxg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yqxxxmwy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zmwhtomg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rmexwoud.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wadrucck.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yoertagr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vszasybb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kpodqlpc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvvcnbn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cznfihsj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fjnwbinz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mkhroffo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3manuxkcy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3olwasmqm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bwucffku.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3egdzphsc.html


<!-- 参考信息 -->