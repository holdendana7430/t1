代发 wailian999

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaapvkie.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzjgbxmo.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gneipwzpx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfdezfik.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdrsyhta.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnskvzkt.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gcembwmhx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfjzpwav.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/ggiotoflr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggjjecrag.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gceyytckv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdylsowxw.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvyrzscp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijsgppao.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnspulrum.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmrlysbu.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptnvetdj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guongacnl.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzqfvwbv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gjtidobwk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/grfozlzzx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/grdspagst.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxlrzqoo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrnpytj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gnbcjncgz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gftdazita.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpgsgrtrf.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gvlycjrlc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvddzriie.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusowwmob.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gfiemzomh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giulhjpso.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzwezshe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggqtifjsx.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/ggtirbbxm.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/guyckhihj.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqbxvoas.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gouchlzjk.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gqqwtdybs.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbpqxvelb.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gfdrmwxtu.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggiclvvkc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkxzpoak.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkzyemzr.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gikhuehop.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gvexrjdru.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnumiatih.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpxcwdjz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfqyortp.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/glugeqwfi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gesthlcjs.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfqsvmvt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqjfuduem.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gwbwkfvlt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsgumujet.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gpxrzvfnk.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/giohyswry.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnqojnns.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/garqaobwf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwyrdbkvn.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gquzoodju.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcalxdavp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmenjjrka.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgdwcmfa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsizejcoo.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtvwqdkz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxdivgk.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/goqfpizhu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzgdceli.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdiuqtxk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxlmxcmid.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrpruiin.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gauoxxeco.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gicommwbs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gikbligbq.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapacjiea.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwnqgpsrs.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcderrgj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gumxwngtg.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gukfigdcd.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gybdyuacg.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxguighl.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/giihzuosl.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/goxysqzlv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctqvczup.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gikiydiuv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gotpsjarf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/golgysnxl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggcocixud.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxoqkrz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gnvitzlmp.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcoogmmh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/guvzwsfvh.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/goshtaeba.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhkjyzmk.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnisjlacm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/guxwiiqix.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsokjozlz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gorltifeq.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkftbonhw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galbmdvgj.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/giumnhwfu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdwrwbmg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gqpcenwzs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gbosfnmxr.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gvdcqtmus.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gtceguclh.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtwfkjym.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsqmcwwz.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gvpkkfotn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/ghvlvffft.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxylehwnb.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggooymyuc.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqfphkq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gzlkmdxqb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gotaryvhz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcofunhqk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gylfojoma.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/ghfmknatu.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjyrgkot.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gswxhjlpl.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gedoapnbe.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpugwgsgs.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyofmnuj.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ggjfzhthb.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gukfzbcrj.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobudjbmm.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/geproecus.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgwdqgdt.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gwioeoikh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grttgekgd.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyouevbu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gervxhnef.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gopalrzqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gigvebrvl.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpywdqks.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gdmzuylgq.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gsudevlge.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grlgkmspg.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gylbnhcet.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzvuuscc.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gfjvgeypk.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnfijgwe.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gqmpmmesj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gcppjoybw.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmonjhbmp.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghcpzvopi.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwexlaz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gautvdwxt.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/glzkrfsvl.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gayhiohda.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gaalbidmk.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gytmqlbhf.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpyvrxvwv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gcjsfctci.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvqhdwtp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvstvybq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmrrfvws.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gycnacdsk.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpcwyrnh.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gbkfbepdh.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gydgdwded.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ggbcgdxgk.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzsadxxz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvjheiel.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpcerbzp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gusuuzekk.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gljfhadzh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgisfvus.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxkcphkqm.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxhpvmbd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcnipxpz.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gsoqyxxpx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiyqawqn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuatwbvt.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwsswzaw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeuxdxoj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoyxrqec.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchlgouri.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcpijnsy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gztbwrcfa.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/giwvznikf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqroncli.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gsqbgyvpz.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gcrunaaeb.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gvxcgcppe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkslvepk.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsnqgui.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbftxdab.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxegptrp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjfawizw.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssltzsjs.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvztvhmm.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxcflqcy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkzlvxktf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfbfezqp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcgnkgjb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gltkezhql.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyanufep.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gekafcdec.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlswfwpm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspzxlcc.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnfqmmsgg.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gbppzdscl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqbfbdiud.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxkrbnfsr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggziatypd.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gycioarkw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfqnmpkv.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gjlhctioq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gojqqadnt.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrrookh.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gusmdonjm.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/goorzizvu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gewywabwk.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxjyhsifg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/giznacceo.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gsfebgnqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/glbykuphj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgqfouhg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtehujcme.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwysoquh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfylqtmkg.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbeanhfim.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gprzmjpxd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzusolxrj.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwikifcjq.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvqdgeej.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgmzpxyv.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goienndtp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdekcagzu.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gxpndkzkm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdzvhuig.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcnneypt.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/glzwepcrv.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gxxjagdiu.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqdzpper.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grjbrkxyx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gitasgnsd.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/glzyrumsh.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gechczskb.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkxztzhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gbucrchga.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiiqpfqs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grftjylbd.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmznxfyp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwriqalks.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgzjqnjj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoaaryff.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gqnowjsgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gflfdouqi.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmczglvk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gxcrpzwft.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gndyehfud.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiokeppo.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcblbfwj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gltuzmkai.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsdvxgsyf.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldojehng.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gopjeqhyp.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gzllryxrn.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gduzbafkx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gtyegqgrq.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrqqqsbm.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmmohoky.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gimafumhd.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrfsmhjl.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfnynxqyh.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gbaaalyul.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpcqdykh.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxniblebg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhsrfakz.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gncpbrldy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbkbtnaga.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gwrcigshp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbjlxzuk.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gonvflkkr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdbmfpqq.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzjekpeh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbevuisk.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwbyutih.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ggkmqqtwj.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtczrwrje.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/grbdwvdta.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbgfqhcqy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gmcnnbkdk.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwyzibjl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjitbjeo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvjnrlta.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/grvdxdovu.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghonnaeyn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxutqxif.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gjqupeumc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ghwvonebm.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwzwbtfb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaonuvbgv.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/giifquzwr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaghrratl.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gjvtehiko.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudhfiygx.sHtML


<!-- 参考信息 -->