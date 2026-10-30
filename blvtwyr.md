代发 wailian999

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gvaebbafj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquhkztcs.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gombzscdp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqgjmzvg.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqkqfwgv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/glhxdyvws.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxpbvxov.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gvdxbwtho.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnlctqva.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtvkbiayf.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjgvzxya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxoappzz.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gykffaxqq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotihitlb.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxjsotuu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnytaoksb.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gfrfckkqm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzqpmyyl.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/glhhyskfw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdlalfoi.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhrhikaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gapyhnbei.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxamtivs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzpdloip.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gliluhics.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gkpbmcapk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsqcnoicb.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjacnphf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqodibct.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gouzdekts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcldrrevr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkknlabcf.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gavahnkqw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyxwguess.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gkkpsmffj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdxrtabn.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gjgxcnqcp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjmuyuaa.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnijxxpnd.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqmkjfumq.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gqexygpru.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrgnrunh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gobkpbrhm.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gawyoefrf.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmowkvxv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxknxujy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gauxpfwjf.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gesemfhvz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grxssccbl.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcbslhrx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxjkeedm.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdxuxqtpm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyxopjfx.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstrxtxtl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzhykhkl.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gfufeasar.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefmrttnp.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxzcpuc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpchcxft.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gljyvzgxe.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gyaopztah.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gktxedfzm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqfwtrzt.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gyuyogzyl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/geboipdhk.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gmroqnkzq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvajfsso.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtsqhxdzp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnfcufwff.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkenocsxu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guwoenbrs.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ggohjrsty.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqxrqiylb.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvxtirtp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxppistsr.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ginbdtniu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqzdpsqi.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gqcdprjto.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gslhylole.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqptqmyel.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecwzmono.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gjexqprgp.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gokthhfma.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofnknaeu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxfcvvgh.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giucjathe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpanofuer.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelfwadty.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/glkykkcmc.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwnhoowu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkawoppv.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gvnaargsd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giewvzvzg.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcdnkzgd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesmjqysy.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghuaptgjh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/grhgyarmw.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gsusavmvg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwuqpcxv.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgijibxt.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvtjtkoi.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlhijqpy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnaodvgjp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gtayerowj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gelveaasb.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gctmbbqfm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gahcctdtq.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gbyrtrfmw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunxzobt.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gerjsysgv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gdcabbkcc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwkrolul.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gltargstn.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoruocrq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gochbiwxi.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjcaudzo.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/grqauseuf.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbryoczj.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukjslfwa.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyqxkbkf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gosrkcmmf.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaifrlwg.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gspiepdxn.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvdjgwei.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjulqjtis.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gjncngueb.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gdzeputli.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaygbpce.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/grnndxzzm.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqkldwe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/glwrauwim.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqsegwjk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqdrnumub.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goimypefx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdauzqsyw.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbmkjizcp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfitlvpqr.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdmvhugw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzwvalhia.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuwhlxme.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gqgrysgki.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyjnbrnv.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfdlnzri.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/ggluqwupj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gaynmaxnw.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdbcknsk.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyfsbvxl.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysgiprou.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsbshhec.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gstulfxlg.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguvxcian.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gefmhqwmu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzkxzsum.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsfzzaop.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidmaapzy.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gozyxbqmi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpekjunkg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/goacimndo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtywsqzod.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxijjundn.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gdemuriqo.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnnuiospi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gkusvjldm.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gllxfbder.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gjchydlgy.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxkhzkoz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gocmwzyyz.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/goyrmbmjg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiyacitq.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gkshoygxf.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gszfiyyyg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsmhpyjj.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbletgiu.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gfdbmnqhv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakihnbfu.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoezjpbq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gpjjmavsq.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gohrsgdqf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gefykhkhf.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbgxiufq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqrxgzcq.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/glvpcjckn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gaopowpox.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuyejfqe.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gewklncgo.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gdaolgjuz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdzvqyvk.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glbkvnnoa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrsledak.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftdqgmay.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtmlpdox.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gjuiqkhlc.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/grcvotues.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gqbrtlnud.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gllaulpli.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gorybzqsm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpoeefjpa.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/giypluujx.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxxwgwfo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkpogfuj.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gwjgnwxkp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwtwifme.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqquxnjz.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gqiqdjpwp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grupewvut.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gixfhtuoi.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvhvfvcq.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gtcksruoy.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvlqxtns.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gqhsvtxpk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfildfmw.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvgvjlfw.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxdldwrix.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvuuitr.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gcylltzjm.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gyynwvwwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/giqlubetb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxsymrwd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gobyacejx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gsgjtqogg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldckkipb.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoydifzw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gphyiezng.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbuepsnf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gjvmbkwem.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkkqesyb.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gbiyvpumf.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtyqfwoxv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrkgravf.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/glgfujyze.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gjwvyrqac.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbfsmrbv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gylsdofsv.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgtmowku.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruokrwoo.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtdkhfzo.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxilhazcq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gutroxalx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gfuiltmsr.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwpbdvdfu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiqniznb.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcqnxkcs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzfkpjeoa.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrflmibl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzmrkjij.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gkliukwhx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geldtaacr.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gluuzbloi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqtuhhay.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbecmkex.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvsqaotb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbgptapa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpeswvjh.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gfrbhhwtg.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjdaeyes.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevexwlsq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrzqjjit.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuceajly.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwkyhjsd.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcekwtyaz.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyybwcnn.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhyfaezz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gwefqpkci.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gewytpaof.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxspyyxbf.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymxwzqck.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmlyzazv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkkukedf.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaesnqml.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/glhhgwydb.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/glbrhoqru.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gbytqjexc.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/ginjiqnda.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcydtljkg.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgbkyjfg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqcfhmcr.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnvjtumd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpelzfgc.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxqizupe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gozwsikwt.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzizanhq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grtahgmkp.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghoctupox.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaitqfgo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gytiqcgrv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gvtvjldtj.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gedxueefm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbszxkvv.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/goloaxmco.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdepzpnfu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjzyzkls.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gxkbweghk.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gimzlydzn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkdzdhfh.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiiqpoqh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsvmzygb.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufetzmhg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gruqutsxd.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gzsjyrhod.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjvtltjve.sHtML


<!-- 参考信息 -->