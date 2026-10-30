代发 wailian999

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gsvlydzfa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmsfmkbhk.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gmuxkzpml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxtzhzbin.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/ggrhcpixf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guyucvszw.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/giybegnrp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghksvjnni.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gmvwxerkv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsbtcxcow.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/glcfdyouo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gtydhbzzd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/ggarptkkj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gniuemvsh.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gvqretges.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/godyabwdj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gdmctdkoa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gehkmqnwy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gsezjblaj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gdogtekfb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gzgbygyje.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gmiduyewt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/ghxkdaqfo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkkjhxqdq.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gtwlvykkn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glikvbggz.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gefltltvn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gzlnyhcfh.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gmbbxmfnq.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gdemcvwdl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gilwnrkvo.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gfqccfolg.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gujbgvhan.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gpzacwjek.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gvvlvrsnv.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gfvtcygtk.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gdnkdsxhe.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/guvxysazb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gjgluvrzk.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gukhmrewt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gxctqhzmz.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gmnxgnyzm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gtwtoswcg.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gxmooqkgk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/giwtfebcs.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmlwnudym.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gmswjlhlx.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gowuikjig.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gxkvvqzvg.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gvvajxwog.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/goxdpvxne.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gojypbnbs.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gemgquzzf.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gnnprsmkc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gcnetxuik.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gnzftpugt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glzqtioca.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gdebuugsi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gjvrywjmn.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gpkxynlxk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gxtxljtvo.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/glrdqgwge.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grqbbvbjs.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/guyhigroz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gmlwsveoy.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gfyzoggaf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gwcxmqzzb.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/grallqwoe.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/glqrafvvf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gumpnmxaf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gguwwkmao.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnpbwml.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gqmhipmkc.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gymzvnrhy.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gkyvspcsz.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gusccgtrg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/geqqtlswf.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gyelvwjge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/genqatqto.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gigldhezn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gfiurbbal.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gltwyjhdn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gdqsuibfb.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gdqsecybd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gdfuhjmcc.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/ghlkmejbe.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/geixwoqfh.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gjdjamczj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gglsopcff.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gariorwen.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gjadqclis.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gnqjxrbsu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gjswnctoa.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gpdlwhwbz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gnatfjgbz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gacsqluei.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gbybksypp.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gyviswhbv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gjdvnvfmg.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gijdduxza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gosfpcmsl.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/glbhgkgxd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gvvpnjqqh.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gilcexfxw.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gppfgfvar.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gwhtolrbj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gtrafoigq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gzjzcqqcl.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/glvwuibvv.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gnpiklbyh.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gjsvfsjpk.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/ghmdikjdh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gwbxqvmtt.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gjqddlcgp.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcyeyrura.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gqqjcbyoo.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gmvvantya.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gzynrznvo.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gavaauqtl.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gzuujeieq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gpaakugxo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gbbstjvqu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gveatinli.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gsrohvfrg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/guzrioban.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gmywvzxjz.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvlnurvhu.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/ghylnxcay.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gpeqzxytx.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gfnkcjozy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gxigqgdxs.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gtaahxrom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gquphhcrv.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gojflorbm.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gdzyqzbbg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/guktbeyzq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gavrhqfeq.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gnlhviclx.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/geqzowsfc.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gtisoozfq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gecniskgy.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gejyejvdi.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gvqhnxnyn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/goftpqrfu.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gakdhqaym.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gtqhqlnkp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gdzbhdclf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gmnechpxc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gmpcrwhpf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/guctzadso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/grlduaykr.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gwawbazla.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gzzlhsgbz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gorqpybwy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gdzhqpazj.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gapbbqkgt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/giomsgihv.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gniwzbxzm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/giazfczlg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gquttffos.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/grgrgczgo.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gvghjffjl.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/geqvztcig.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/guugohvhr.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gjaghhpeb.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gbfvhxkob.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gnkpnmazr.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gipjpyuws.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gsiqhotpq.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gwzyyvvgo.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gqqvplulu.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwpxnoray.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/ggfhlnnpt.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/guccvhsxw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gsiycemwa.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gxccjfskg.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gbpzzhznd.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gbckjynyz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/glraiwtqw.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/guutmtfuv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gkxuassmc.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gkqnfhsda.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gtotfihbe.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gxqndtyxt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gjdcdwsbt.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gdmwipzzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/ghqvcwopn.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gaxjsmask.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gdacxfgjf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/ghcbbejfk.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gkqbecxhd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfypyplpn.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/glglzjxkm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdvxqbqjv.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guldmgfij.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gvoqaandp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gbxzommcs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ggabohgcr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/godmgdbyh.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gtscvnnoc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gtmytvrsz.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gvawtfmjw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gsxxmqxvo.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcjndcykx.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/goloibeol.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gupnuvsck.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gevfsxwld.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gcfdebgjz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gfzeacicn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gwwlznnwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/ghzugyhnw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gepzhjztu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/glyhkflfs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gvbncifbx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/guyanhqwn.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqeaxpjtw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gejaonpyb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/greisjqyb.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/grwxaqmnt.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdrkazijl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gnusnmwox.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/ggbrnuctx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gwtbpahda.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gaaucqywg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gkdgdqmxc.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/glqopuhce.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gfplhandb.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gcxylgwhd.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfrgsjfhs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gffllgmos.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gcmxvjlim.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gvstpubeg.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/ggroztpvx.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gvzbyydjk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrlbcbh.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gdfvsrimq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gjsyrnymz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gwcnfyknc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gzarqrafm.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gdmjcqfip.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gawdlhjpa.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gfddupurt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gnbcdlycf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gehrtrloj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gcrpdvgdq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gqspwwaws.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gmvdemtco.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gkiojpphh.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gckdrhtoc.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/ggmsloncm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gptnbqhfy.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gweexckyp.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gontsoiyd.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/glwuzkrlk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/grsderkdp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gxlkofnsb.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gbagpijyq.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gqhlcbebm.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gkllignvi.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqdizqpzc.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/giahtglqw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gnmzqscmj.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gqiqcfwgh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gsidhgslu.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gifpxnxjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gblnyabzt.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/giyjhbgnv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/ghmhrqcck.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/geobfdcfk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/glolyuqaa.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gsszymudx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gvqbigako.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gybhhawrt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gqgfabnmt.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gytlxdqam.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gncelwqzr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gogpaciis.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gtlruiamm.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gvkoaegkc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gxngepbmz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gbbscdokm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gxjkynwok.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/godnrveeh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gjxpscxqh.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gkwdsdwkt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gprfcvlzf.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gvjbvtczr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gqavbivyf.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gkfejrmcm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gnzfprikr.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gacwtknot.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gslsgqafq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/guwicxdvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gpdtggppl.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ggwjqbkpk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/giccrxeds.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/giazerlvy.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/ggbfburpp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gntnrxkjf.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gommnrqlj.sHtML


<!-- 参考信息 -->