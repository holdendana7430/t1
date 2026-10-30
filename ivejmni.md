代发 wailian999

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/guakygdby.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/garwdtnzj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvrfydlg.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ghajmbbih.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxypqgzt.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrjrkwdv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gpsyeudhn.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/goruezbrj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuwszexu.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gehmuoqmd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzkfjuh.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoqmjumm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/geokahmdf.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkshzrht.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxngunvl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gmolkohch.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gjtpjkadx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqdvigdh.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezhovclr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxmytoyg.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gstzdvngm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gtviudobc.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/giddrzlaj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyduyohw.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcxzmkwy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/giztebgvq.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqjidjbw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmlmlwfu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqubdiai.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgfwgmds.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfoosxxny.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gogzqjkcs.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gcklizwnz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaujxzgew.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gyuwsfvex.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gqblrkbih.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosgwmiyb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gczpmwzpn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gsurljdac.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjptsyjo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxffktkb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gzdvedivh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpjytyecl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gxksdkzjj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gehbhkkdo.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gjrzdnevt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrppcrcq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbpkbppx.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwukzuthl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grldzfftr.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gptxeyhch.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gzstypvuc.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/grsalmxjb.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gvdjdxxqr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkunduzg.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrzdyhzi.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gkbnurqgr.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbtfeoisr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtclhfgac.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/giiqvtkvt.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gugpuqbia.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukdjliab.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvraglnfl.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghiivngvq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfufatmhc.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhuuuvyi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcxdemitf.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsqjqprt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkjrncky.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/glfnsndyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbkwpfnb.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/grqlekvbd.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzjywmmd.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjkndpzs.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glussagiv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyicrsdgl.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gfqegmebz.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gixqhodwe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzchvgotc.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjwtomum.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvpxnmds.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/guwumvhcj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbsphvtme.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gegyfcchs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggxudgfp.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggljucgkf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxlqhchpf.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gdouikjar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhljfdtq.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gkydmkvlk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqdkcjtd.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gqpnuwdtg.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzioanxso.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqucycho.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvlgdpkx.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjqyragxl.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gayxotibh.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/giaouckwz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkidupaq.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmrxkewl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsiwvhune.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxwiabbnk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpvicbkww.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gjqlekiwh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghqtqppik.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/guynhocct.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxpnedrm.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiqrbgqu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnbyzhsj.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcesldlxd.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfkyowle.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghrkvnyxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwiedopm.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gaodmsibe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuviflvm.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gimsarkwf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gezxsaynn.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gaokitbfd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojekelqh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzsmuzqi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdpfkqig.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gwdfgcozf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcqwerut.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/grknysnug.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoogwfaf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgwnzerg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gsguqxtmo.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvpftnez.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpaqnued.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gkkfmmizh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgwpjbkg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gbhjjitxo.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqkasnu.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpajybgcz.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzgbaghk.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdovgbjy.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzamvza.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gnavfgogk.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvfofpcwh.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwyanywe.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gafnthvvj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaaowwoq.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gjhopkkfi.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbctroyph.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gcnygnnfo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/glwehkfli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpsbewue.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnenrmger.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyowhufqs.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gthuzzqsh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grsgacinv.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbddlrnzu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gjgnrooen.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpndzsfyk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjghqzbs.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gfblgjxgb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gactgybmj.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gchlsxnfz.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdztywhqr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gppzafgwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gnembdorm.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtttepvta.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkyimyxy.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gxzgerkgs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gbmhhscci.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/goyofeaxz.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzhakrdg.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuyrdxhl.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gxgwqrjue.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gicrkytfr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhhwzfxx.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gdhbjggfv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaamyewpe.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ggqawbnep.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflgvrgqa.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gziajwwfk.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gtmhlkfjh.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjffpdk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/ghbhjplfc.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfqthjlv.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gzamctuuv.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gsjgnszjr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gjqldefzy.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyjtbfpzg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/guubvjimt.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcactssdg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlmhbfud.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzysdutaz.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqexwypv.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/glxhxevjz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gctbtjxyh.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddfnojjo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjjzulrv.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/grwixumve.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gewbwcgfx.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gedvfuytn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gjizloaoe.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyhksgzp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gakzigmgl.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdvszamhp.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkduaqbu.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gmmokyowy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlrvvuuc.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtraikhru.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gdcgsapdx.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqqohrpj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfynlgjou.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhbpcqea.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gnqdspngu.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiwzkkta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjoedrnlc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gdptfhzax.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdocniolh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkyyjrqy.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gaobtftnm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtgfyjfh.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gntkmcdfe.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyfvlorr.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydsyprtd.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnpkrkzw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdxhhknt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gildhhnvx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbmudgch.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjtcunsb.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gqzpkpjzw.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gisrjagdr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/glwtlqxtl.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbkiltwbp.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmvbvxfwa.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvhymtgg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gbgqfrwld.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpvilajnh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/grxxwnsob.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gopabeffj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giikncdeh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/grpscjnuz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqskkvixz.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqhzhois.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gselxjzge.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfuizhfnt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcbtqlxq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbramva.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gyduhmlcx.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/guietdxjk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjysblpcw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gludtlvzy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklrufboi.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjsoyasn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzlraijh.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxprvjvmf.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjidkshbu.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gyhttdxdr.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmmkgxlv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtdcslfyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gfftfiyux.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gohlowbjv.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvlckmih.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhuxyibe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gcwerioqx.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcsmhekb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gttwbpnoe.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gkhygnapd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gntvgfzkx.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmkgnspb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoyafkvv.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/glfpdsdzq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkxjybim.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjavbicn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gmlhcfegn.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/guevhrlml.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqlzntbj.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gdffmmskw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjoducyu.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/giohtoiro.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gtakkmkgt.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyepuhabe.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggckbkpxn.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcmlqhfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbebqnrtb.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyjidqge.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/glyoqcize.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gdgilznzg.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gmyvlwbxa.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwdfmixzf.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkwzmjdi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwlgkxbeg.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqrrmeux.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gvorvlhuo.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgelaalw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gedithbgj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/geitzrbak.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glohbsecb.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gkbgklurt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnxbexgdq.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacxjxkxo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghejtsnjb.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhbujogc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzosoqlcx.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdptaqax.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/garixwzdy.sHtML


<!-- 参考信息 -->