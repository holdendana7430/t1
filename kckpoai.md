代发 wailian999

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/geckoxpym.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gbtrphkdu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gxjgoclfi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gjrsjflcx.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gumnqtrsr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzjjznonv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhawtxl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmjewhxiu.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/givremmid.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzibgrrh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkzzhevbf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvqyfbbfh.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gpedmimrk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnrtdxvvl.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gxeoatijj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gbzkfnxyc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gtknfyeen.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gpubfykte.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gxvjsdeek.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gzhappthj.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gdprcomxq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gjqzinaqv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/glacinlib.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gsrxqyigk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/ggvbxkylm.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gobgptgsq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gnqrjdlpr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxksbpnxy.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gvmnkybml.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjzbxqfhc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gpnzqheve.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gbtbrutno.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/ghjzlzolu.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gplloggqm.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gmdnmsdlj.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gnaxxuiwc.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/ggaolmabx.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gpdjqedxw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/ganohfiwv.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gebukosgg.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gvwjvvldm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gkyvypzzn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ghfzsjgph.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gwpuwrizg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbasppxcb.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gmplftoum.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/giaxxolsp.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gfyjguxlf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gzxwlynkr.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gmsvzuxtp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/goqjdamgl.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gwhfejcav.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gmxlfzrsv.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gimpvxpqd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gcwwpgbfk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/graviycxv.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gjpvxzqrw.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gzgftbgim.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gtucaheqc.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gltpvalgv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/glzaiqhvr.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/goifeuscl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gozdvomfs.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gkvviiwjx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gnvuwinug.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gkhpdpeeg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghvlsplrl.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/ggscnlzsi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gfqiwajtz.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gzqmtcebr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/glhoayjmb.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gwiwuywpv.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gtwvftnnn.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gyyoaxgzf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gdqjllggx.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gjcrulyen.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gwipurviv.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gddpilxtf.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gdxrsumbt.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gnqzmsdbl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gngiqsoqb.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gmxndevnj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/guiieiuun.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gllouyukt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/guzukafvg.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gyasdpvea.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/giyyzjkyu.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gpmzjfxvy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gpbqjrbhs.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gvpzxpuat.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gncepslyl.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqqfhrdyy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gmcnfeuif.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/grkjzghzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gfttslqpb.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/ghbijmche.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/genicbxuk.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gxbzkoygq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gixlbetqc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gjcmrtujx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gqytprsft.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gthojwrus.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gytsyrthr.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gsopalpit.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gltwszpwa.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gtuuursjx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gzpsguzfu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gnowrvtwx.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/ggsldgbct.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gnlyvvwji.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gyhvustul.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gyfqreywu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gcajpttzj.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gkbfvxsbc.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gcpshrabd.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ghgtnttmb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/glnjucsci.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/grvmnlqow.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gsgqmzoci.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/ggirceccg.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gkgrjcbvb.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gtvtmrptz.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gtjxomzah.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gmpcmmzqt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gtksqoihb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/geyizlciy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gwvqmebuu.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gwxrmsmgb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gsyyzprpn.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gunvckxwv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcwtmdksx.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gtzvcjoxv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gjonaaxww.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gbsdywlbd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gchnyhefl.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gbczmqljr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gladyxwop.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gbalpanui.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqspptzov.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gqnlsipbw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ghvuwtlir.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gslaovdxm.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gjgwwhxww.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/graduerwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gimevkwzj.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gogntmkky.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gjxccbpjh.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/glsawxbyu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/geupkxfuk.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/golugykcl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gysjkcaoe.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/ggejhrgbw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gsusonjzt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gqqmunini.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gjhxwutft.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/glehtporv.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gsjvemmbu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gebwheyas.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gsjvirjff.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gwosdeewo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gbcvglmdn.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gqigsilcf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gururperw.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gqymdysjv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gklhtjxqu.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gvyvesffx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gfontosmy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gspngvoim.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gpoucrmxz.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gozayyxih.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gueobghps.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gnefdtnvs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gbrjdrtkc.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gmqmukvhr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gdlrgowpd.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gdxreszot.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gfpljhsxn.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/ghtdfmppm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gmdbylyii.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gzkcgxuvz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gmxvrwyrd.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gtfhatcwd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gkkeqaycu.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjfssdnzn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gdqpsjvvw.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gymprppud.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/geznqythe.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gmvipmrud.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gtyhmcelm.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/guxudaedj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gzvjwcbtu.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gytyyppmr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzzbfecnl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/glcyewmhu.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gekczzwyt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcybsecpf.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gagfeeclx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkbzfepwv.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmmgfwwru.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gbizkvouh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gmhjjxnow.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gwrwedwyk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/ggqjbybso.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gjpwvwwjz.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gjvleetvg.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/grahfkoro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpkqxkhfu.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gwlyzdafn.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gahnldjqi.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gyxmvrxel.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gtynsjuwf.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gjygiqxqg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gsvuoenam.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gvuqfiwgd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gceitulwb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gqnhkdane.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gisijsjih.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gsyjqrpcb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gnxsejowa.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdnyclnvp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/glooicpiw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gpyzkchid.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gpybkaqiq.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gebntzrgj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gvxhourkt.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gamuaomll.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gvlrfhlyt.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gaofiescq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gjnfjezgm.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gghwmiqoz.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gsddqoodk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gfhcbqzpt.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gbuipuuqq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gberckkrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gxebfddqx.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gpxuexrfj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gzkraazac.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gnncuzxcm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/glrncrydt.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gnnvdyzba.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gzesrpcpo.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gsdthkrrm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gdxuerrrp.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gmohfbmfz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gfwgxprvf.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gvakynrwx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/golstfcbw.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gtxgfjhyx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/ggrwatpmm.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gdhtnyszd.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/ghxldidgh.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gwqnmvrey.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gklvihnpf.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gdygnguam.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gifahjxzp.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/guqeqdhvh.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gydogotyt.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/ghiycswbd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gtswhqrxd.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gknqxksqh.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gbwlfbroj.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gaoiqacfb.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gjglshkoz.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbtxicpnc.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gazcgtgdp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gsvizvcbx.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/ghcccuxqv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ghckqekyq.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gargzyfsg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/ghnmbgoas.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/ghbibokdx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gbkejrgqe.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gtejxzdsu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfmyrcpbb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gwnzrimwo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gxfabkckt.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gbhvajkuu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/goucazgij.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gbeqswlfr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gnihpvasx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/goevtsgur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/ghgqcyvls.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gonlnwflu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gtoicdpdm.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gdikaudmn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gfktoakri.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/garaasmnr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/goizotzoj.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gqghthmgu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gxqanpfnp.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gaqdfvusg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gpekexdlu.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ggioapszv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gjljfxwmj.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gtxjirdsp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/geprhuffh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvvuqapyw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gtvwddtjx.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxdgvhgyi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/glvyapdig.sHtML


<!-- 参考信息 -->