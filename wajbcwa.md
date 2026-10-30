代发 wailian999

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gezndqjpd.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/geqqwspbp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwvpjkgn.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gziqwjfqj.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmpruomed.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gotgaowec.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnywbbiu.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gycajodre.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfwlrdqz.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gerbuwysy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/glfmprulg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqcibvjt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztdimsof.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnfxkebsx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkahnzjjd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gyvmolgnh.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeblhtqf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdqhfyiv.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwddseyjf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gljiczjsk.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/ggxslrhsn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzgvdrwg.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvpmuamf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxopgsww.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gcscoxkax.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzultcaur.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzouocwnt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmibpnva.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gotycibqp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpsheeqqi.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpepvfzi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqhwclpy.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gphtkjsap.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzdgqmew.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gmegtpvbl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gbzkoxobh.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gbkngwgnq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnuypqpq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjbyovtq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkobcktc.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlqlxggx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gdwoqisso.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdssakxjj.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gdljcosuq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/grkekssdi.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gpfcnocmd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiixzmsv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiavapef.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/glceqsmek.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdviuanem.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmtrylcy.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gkykljuyp.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gankszjru.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gduuojugv.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaabmmgbl.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiyjmhbi.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gdxvmzuix.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmdmlmggg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gopacrjzh.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqyjfern.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyckivsy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvrcqyxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcugwdaie.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/grckboxzk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpebjzfy.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvmennt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrzssbwd.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrxvepep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glgyjqibu.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonlfpige.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfosiawro.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbhemdwe.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/glozepfhe.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gbkdshasd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjoirqui.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gabvotuvf.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgrhxtni.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlwnkwzc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gosfhbyla.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxvgztgx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqacgmphj.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gvybitfho.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzztbjqim.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyjwdaqr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnlkvnuww.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtqoousj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzjgeitr.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gnalbplpp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gucisrwje.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdqafmhq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdxyunde.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjjqcrecy.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghaohjgjw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcchtxfg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmstdwiyn.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gminhjivu.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmqevwxl.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gutonrzvi.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gisczzeam.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/grdnfctqp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmxjecwx.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnulgwavr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbapfvqb.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzojgdhv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkosfliih.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvnnfrdp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqcoytyo.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoftbtax.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkdfwcji.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gefnshatl.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/geuguoxdj.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/genyvitis.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/giocpqlrz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfkktbsl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gudrrgrkb.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqnlbsesd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqfeqpbv.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/ggrrkdcah.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmwhxamg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gwexsmglk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gphcdoxzw.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/grfuhvflq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/glnoscofq.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gkgbunipd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gbckzfkgn.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmvkbkfes.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gvhskpynf.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcieslruy.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpcqkrcis.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gicusuzos.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrtufzip.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gchuwildu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkviqspyb.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/grvkotckn.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gcxgxlxlj.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gfsiojsyx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzjofaufe.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnnnmrhp.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxspmqlws.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxafojqlc.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqlfqrna.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzhzbkhq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhgughop.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlcfkcab.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/glrxczlau.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/glvqfqbel.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gkwdwgrgb.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzcsipbdl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfbnpaqbs.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtuqiqvz.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gemhawvti.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxklhsyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gjqzkvvrj.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrjclajd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuyhmieo.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjbckhpq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrnpotgh.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gsunstabi.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garrtdwbt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpmrglbw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgxnkkei.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glfrplxmv.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkktdjlzl.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvgtsfqd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gxnbsolrn.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqarnshby.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyuzozou.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gvvlrgyxc.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gatmsigla.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaxzhxlv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdlwyill.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjrfixhn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzgvsrxg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gmjkbbtll.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gokfkyuvt.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gczbdumnk.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsvwxrgo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwovvwwqz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gvimxmehx.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaczwdcq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtldmboa.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulgjavnf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/guovgkxxk.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gnqytncez.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfayudwh.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbkvnta.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/glqalqneh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyradmqnr.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcafixttv.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ghenbangf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbndnkemp.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gpyfdafgc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfivpcyee.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gbfvgmlun.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdcioepb.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdizbavyf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gefjpxpcm.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gxyffaslp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihbjshhe.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/grzkncylr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrkbimnc.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxhsflnv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/geptduvue.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvqqkztu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gtaptzvso.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsllbinwg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gbzdqkzhf.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gaijuvuel.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/giupjpyex.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gfbmogmgn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnkkqxzdy.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gwojmrxzp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipkvrzbh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/guhmfivqi.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gbxakkkyv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwzwwzmv.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gstapnkkl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaywbymlv.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grtigbeda.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gazqzmloc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzscmusn.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/giqhonosp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtomhfoj.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gbkcxhlvd.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gopxmgbrn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygkwgizy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyicajevk.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvvbpmcd.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmjanlzuk.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gotpittsp.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvxoskdlz.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gofcvnsso.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gutrtzlmw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gatfhvfqw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqhkeavd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ggezvmjkz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/govgyasfj.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gbtbcisia.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulkhoikz.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrqnscds.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhzkzpxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqrsqwgf.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyksgucc.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/guierlqxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyilwftmo.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gtdkmkqwd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/geqdjpwln.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdgrbmlp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpazcyrzl.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glebeiomj.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gdyzqlocs.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwzmsqtq.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glygakovt.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdxmgdfj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkpzztip.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gowpergcp.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gxyporfgs.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/geabkgnsd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqyoqbds.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gazzeeqyn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvlbrjjnf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiwjqamx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeykxgeq.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/goueuwhdz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gforwtjch.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gqsmkljjl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqidrybo.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gubenmxvs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggshtosts.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/glisnamle.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gfnwnbxht.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gkzuyhkei.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gdpyeiont.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/goxpvqvox.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gawwevnzh.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gixkzyygy.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcfzmdic.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfwgfpj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gshpfbqpf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdklxznri.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqayryk.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gaxhsczpn.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxgecovb.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glyoyjbie.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gokvcwcjv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjthmiphj.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnjzrvfy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gnvhiryai.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gyjbckktu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gfijdznyq.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gictqlbwa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grunygdys.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gwevudtcb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gonybrogb.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtthhigdu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiupbdgs.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyqlukzr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gsbqobnwm.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmvpvhwny.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gstymwqri.sHtML


<!-- 参考信息 -->