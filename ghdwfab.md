代发 wailian999

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grjmrknnk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzzvraxg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjcobwgx.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtibacjln.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gafygzwel.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwfmzhwto.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnrzvzgvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/griiorbow.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdmugze.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynjyiuce.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gwazsxxbt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gqgdogvga.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvndaoagp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gtpaaspfq.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gunjwfkwd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gelbqogmu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzemjnspd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmmumsje.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gusvjrkaj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxjubanq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfttcjhbt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzomkxsee.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxmrvfzr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxoeezoad.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/grleljktq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrxvhmtm.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfokjykp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnsfxucn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gagkpxzmb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gytxbpzhm.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/guavlizom.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gsougmqmq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxsewsks.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gkfbmkvuh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmxngggl.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdetkvdth.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gtchhvhfe.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsyyqnjf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzepqsloa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgntelyy.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gwvnmqevt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwdcmrys.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcygockci.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gfepihkra.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqaklpgd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlsdyfum.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gozdweqct.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthudxpmu.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gdueafoiq.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvdwicne.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvxhvuzp.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqpppsio.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnfdfwua.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtficgvfm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/guucgjsuu.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkasyvcc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ganwmojbk.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gixgdjldc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnavgshpk.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpeqaunpo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gcyjecaus.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/guvwytahi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpjexdrpu.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbutvnayj.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gkydjcgrd.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/glgzimasj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gaeohlfjp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/grtjznljo.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaqifjdo.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkmdaxyub.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyxvefhgk.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvyvmptv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaypmevwc.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gcxsslnex.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gflfhkxek.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwurnullc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcbxolojw.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gzjscaqqn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadjbchtu.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gayudeezx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gknsdpepo.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gugjpzhot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmxwmghba.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcvnuvpp.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtjyjxkeh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goevjjzkl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gquqmgbmg.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqyqgrqyb.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshteqpwf.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gnvnxlsrb.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gifvdmvxl.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkucuhngv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gztinxymi.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqoyqdmd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphzerflt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gebwcufsu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/giwwsford.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdihjmjtu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmfhoivw.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/goodmnpuj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gaczgaybe.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gzledgpai.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkjckgoo.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnfjrjkfk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvwqlvyfi.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/goeapvlvp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gypmnijjg.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcumdriq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmhjbpphf.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/grjyikrph.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gauqizapd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gjufotpio.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvtljab.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxwdijkp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkbdhvpx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgstbhfa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gzymkknus.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwmgikkd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gjmximgnm.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gltimdhmg.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcwpcgav.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gdqlcqoze.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gotxlumkw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gkqzjaljv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ginpckihw.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqqnswqx.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtvooyjx.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpyujqzoj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvucnhkqa.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gcdkshfuc.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gijdgcuxq.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpwprbwvy.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gogtxhftb.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggczhvtzm.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfplxowiv.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/guoetfifa.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/geetbtiwo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gamreauex.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gccfrknwn.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcdzbchr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkgcnowfv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsfvfewp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwowogcl.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/goenihjzp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gtecdangl.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaufaalc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyttzjcl.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gzylefaan.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbmywobd.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/grpfkjdft.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnnqlvpd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gqunewvtf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gypqfyilx.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gngoxzwkh.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gchwxofkn.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gajmzyyxr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gxdvfovrf.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gutdexkry.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/grouxvxnq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjexssfw.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gksekrcle.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwmvimjqf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/glairqzjl.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbzzjkubd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybrwsqkz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfqfuidgr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/guipaqdmu.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gaxazrphx.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoureakd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gntuenlsl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhtjhpyw.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfqzbtlh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahojydpv.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gzfdwjcol.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcpzjvkp.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gprrtkuay.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gyojwbnae.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuaharhh.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghchyatcy.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaplvevk.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzzqubae.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzomagunw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkxhpbwfg.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gnsuvvrjy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gubahduyb.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuqncjii.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gczitrqxl.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsrsjyhc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjyaxpal.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrwbjrte.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpzbnvjq.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgtrshvd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdovhmadd.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/glkflzahq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwojnuvnu.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnjztxqdz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzdnlpjo.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqetlbph.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnddiubdh.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gegzscqfw.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgrsavor.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjjayqgu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/goxbyskna.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoajywdx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/glwfnmgbq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqitzzcr.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gzthcmvtb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlcmcunx.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gdbzhooco.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxqqmdkh.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gawofgmta.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gysbilwcl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcoprozlh.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvpguvhi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuyumkus.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjnmwjuf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gudlyiagc.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbmvotcj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gxragoxvo.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmtozrmu.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfqecpvu.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzbadnzup.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzuhtsbm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajwwhic.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/guobygezk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdaqyhsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gzmqfggjv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gqqszyubh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/glchfaujg.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gepbgphte.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrfpzrjp.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glihgnpeu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gcknbzxfv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnybjtcdm.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glxiwbltc.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gghjyhrcp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gqeyfjknu.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gwamqcmlf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzbcjchh.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhwtgbgo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbrwjsu.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyckceov.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gccbyamiu.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcoatgaf.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaooljfu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkfoagig.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gwwwzguxs.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtousvxz.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyhsazze.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpludwefy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjqqwszs.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkuiphca.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgrpgqag.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gskndccdf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/glntnnhua.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuarxunn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/geatffqfn.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpdtvlxd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbptsbyu.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/goznbkxse.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxieapzhz.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnoujbdwz.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gulmesvcy.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfcjvkky.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gqvmucgzp.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjvetefw.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdwsfgpv.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmfrexks.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrqefrmg.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcsyklmr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvbxbpm.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gmdsevzrg.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/glkywztud.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjyyhxjw.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslcvvryb.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrsxpcaq.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gynadmevm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfavxaucc.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmgchbip.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gmohdxevg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhudgmnd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gubxikcgt.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazydgpci.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznpirxvn.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gluyeihvq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/geitiqpid.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjzhykbf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdehghjhg.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gjvprqpoy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsomgpzz.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpatrtft.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gbjgabmsn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwogzbnoa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gboirvvjl.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpqhavtz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glepzexvk.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/grpgvftqa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwusfhcj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbjdopyp.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gjhpzouuo.sHtML


<!-- 参考信息 -->