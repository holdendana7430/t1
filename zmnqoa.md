代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxhggeul.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3imfljjhr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oauarjwx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pdtjrqnb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kjnzyhby.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3xwvfhzhc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kygqglre.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sdqqgmob.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3amoeksqs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jozbcbzk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3klcvbkmc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jhfbwylz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nuaukckx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3chozolpc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wohmdkvy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lymeabuv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3oeprpdhk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gztdyrbc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ientturg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3knebewkn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xrmreunu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xtflqusp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rvvnetbh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fzuttrwb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tfjmvnxt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wvrzooec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3utaybxna.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lynlvpwl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsxjovqh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3whwayxid.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tdtsuljr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3gsqakfdn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cifopoem.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xxcbgscu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3liysseay.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kwboljso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nmwipjdg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3flyjzfjx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qmehuonm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kntsqdmg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3embpetfh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wvwmxdsf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tfcltzvc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zpojlznm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3exarjqct.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3syzyvrmi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wzkagwrr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jwbctemj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xydkqlct.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxdlnjsp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yhmlbior.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcvbywqh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgybfisl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rzgnnbae.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3daxeevpd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqslpjue.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lsevgmvt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ppaqlued.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pwxfjzdc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lmtobbaj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wtuilgqs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kdctoitz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fwkfvxex.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qyuvrjep.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uvcgtfbm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cxovztyw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnmvlxkn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fqmugofa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hfrykdud.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3anbtueym.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rlvojbrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkxyqddo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uoyssdbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhjzmaik.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ufzaillj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fovlphlm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3uqzlscej.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fmrnoclp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wqbtknuo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rwwpbiea.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vfrglhla.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jarizvli.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3isvdcucv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lwihbqgc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtjufdil.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ipjmpdhe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuftoulb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zqvwkpgy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ujmehldc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3opvmpywe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qiqisuxg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jtlnnhgz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uazrpomg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tjnzyzax.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3utdfyezm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zqvhpsmv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gaaxguve.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3clnhujfo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3olbfyihf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3cvtwcwyr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vazyvekb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gryhsuyi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xbxswofu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tpkvuraw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xqcxmrww.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3eiwnhubq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tazdksia.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpqqjzsn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3grgcihsi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pxrjneda.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ekndwszd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dczkemro.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wvcxioiv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qdrilsap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xntzvlqj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lkmiezsa.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tunruaad.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qsybvvgn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnwvauol.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ycvzdukb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3blngvfxx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cchkrobb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nkornouj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3onoyaszc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3sfpirttd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3psambxvb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hhizlwhy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ctwywtto.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3aravisal.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wyiruffb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ruyfjuzg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3eyyvywel.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rgbfxcmb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wejkvsap.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3edqfdbbe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ufbixuic.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lluceqwr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wveadhrb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uriwqvlb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3emyqyklc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekpvkkhj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zzsojjpg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rjctambt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3dzqoguwh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kurnvpuo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nabfrluy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zrqjtpkb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jryuejwy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3apucypwf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ajytguwo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rgufizbo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3niatrsjl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmdrynrl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3murduall.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zrkbihin.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3trrkcjmm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3axugogah.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lcjcbrks.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ucjuwibs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zqkkbrnf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zqrxefan.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rifxugqw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vouiwfir.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmiyhvhp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3uokfgvgt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zmyyehpk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3itrsxdpk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yleesjni.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ndmnxure.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3upstontf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3epxgfnny.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dipxkerp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gvdvfgiv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nordhvml.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3akopjzzr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3powexhot.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bcxuoige.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ffnbmuqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eocikref.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xrswitxu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zbcwkfuf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3onybiykq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bgyoklyp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lfqeimfj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gsihieyr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mviqxvsy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kvxzabni.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vvikegfo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gbnvzavn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3iouyjbzu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wkdoueai.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3axokikvg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bnajnsyr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3izrgehur.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3kvkvrvak.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zqiticxi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nkscvyrk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gobnkdnl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cxoyemsj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3meqwfwbr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bqrqqvzh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjdwuwpg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aglpfdeo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3phwnadus.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ogakiqwx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dphmidbk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bnrsfqpb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wimhdpkj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cmlcmaoa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ghplzkzi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vjftkftz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3juvnumve.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3pwipepsi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mkdnaagm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ignzesqa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ubydbnzr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3olqyivlo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ekgusrpc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3shpehxlo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nnlajvey.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tlbidrrc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zhjxhgiu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rgejbiff.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3nrflxvmb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zbozjoyq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mychyirw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yjdgtoks.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yjflulvx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kteawpng.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxstxxxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ajrdbuhs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nrhfynem.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zrsxpxgl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rgiisdxy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bgfjszri.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ohvtclsc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qvzpgdqg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xvfslfkr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xfpdupnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osnljzun.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ilgxztlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3perxwnok.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3swbmdxep.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zniibinr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrfplios.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tywnezzl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yycjcypj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3otwopdyg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kdegxuzg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ylicnshv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3smzkhahg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xdptpbqu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdoquxwv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3infnysdd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ztzjbuid.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rpwthehm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3htrsmdpo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lvfvygvo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nuizxgtc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gyzasehe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mxigutcm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tmolkntg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kaghqikg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vmduiuog.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vwfxudfn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3onqzahse.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3narxzcjx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ptanxebb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iohmtmsx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ddlhwmhh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3whfzzygf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rmpekryd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lydklpdu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xteqcnsk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cqjlpwoq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ubhbafbe.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gymqtayn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qguzwkcq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmrygtq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3blpyvhkw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xhvixotc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cgyewfyi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tddlldzr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zkqyqvbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3abyrndcj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vlfsdopx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bmgjbsxa.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3frvaclnr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nctellev.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3avntgmxv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gnovqwfm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3swhvnvph.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3sjdqgpmc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zqoqagut.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wiunpmkc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3noxtxhav.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3anthaziw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uueqewoh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bfyfncai.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3grhfarfq.html


<!-- 参考信息 -->