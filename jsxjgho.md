代发 wailian999

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gxrwqhihz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grhdttagb.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmsuqnwbz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggbwjugck.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/glefqkerc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwwomipgd.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gzabcvqvo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzmqvtkzv.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gtodbpsli.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmikgwpev.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gkahmstfm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/ghagpphmc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gdvxsmstl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gesmoutyb.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gdkifkhnp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gizpxnfpd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gltjarmpv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gaagikkyr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghjuksdas.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gmqezcffl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzydzvjdn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/grvzlygnl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gpzmwzoqa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnwuudimw.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gonsxclnz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghzfvjywo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gtynhnunf.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gglsxofrp.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gvkxcdygc.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gsjltatrq.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gnhlxawki.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gghrsesvx.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gcmydfqdl.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gnzbkkwsu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gzvmwzhfb.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gfvzzsnja.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/ggrmsrtoo.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gvpmhepzo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/grxljiued.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gvbpxangx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gjhpfbjqo.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/geygksmpj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gyevhaygb.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gjfnmitbc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gqzyqaiun.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/grbosvjjk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/glvzzpcai.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gzrmlvaxh.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gvwtjtmuf.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/grymkfqkx.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gbimgichx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gcekgrgiz.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gpieppobx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gpqdlcycl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gqxkzvhfd.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gtcimbokg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gbsibkwmx.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gjpksmwdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/geghnopgg.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grmmmnprq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gqkqhwfjw.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gjfbxmxbb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gmvxhyehn.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gazhserns.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gusltjaid.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gnkblyrad.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/grbolbrvz.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gogqcbgvr.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gsmtyjtxy.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gphhszcaj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gwrlpjgpk.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gkhwcyzxr.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/ggrldakok.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gyectaqqz.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/ggxdyucpr.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gpnkqjsef.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gqgsmmhic.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gowfjaerd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/geciyvgdf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gwhmzvarq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gxdnkffec.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gkduxemwi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gvxhbfrjo.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gfxwzvufh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/geaxfypve.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gdozqmfhg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gkphslbia.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/glnsmiexq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gonqoiosi.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gevejqsoc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gajjhukey.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gdsmmreyc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gehdpapkw.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gtvevjvzg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhszuut.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gsctnekqv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gfqhyzqbm.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/godeesgsj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjebsgzra.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/guiypejao.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gblsgykbq.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/glqkcrshr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gpstrcvkx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gcislhtlk.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gizcfirke.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/ggxkxktac.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gkanxotpv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gjmhdkppe.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/ghmputwav.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/galzexrpa.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gvcmhhshh.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gcyfbommz.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gheyrbges.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gixylsumu.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gscbnlsnq.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gjofbtzpr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gbhpqidgi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gkvqdtrsj.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/grvjxhjmo.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gzwgtaopy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gesmkfsyu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gpkqrhtbm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gsztqffus.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gveoowtqh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzlzyesdb.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gbrknoxos.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkctittdx.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gmocjwbir.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gkdocsibx.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gdfjrqjad.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbrmovlua.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gwjytfmxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gcpwdorli.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gsqpupmme.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwlpjogfr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gcputlptl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gkoiqwonj.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gmexdqakl.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdktylvgs.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gkpqhzwyw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/ggbjcquru.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gwxyvhhrm.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/ggueidrht.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/ggetsqvnn.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gkfwlgukh.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gfvtjgngw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gohnumwoz.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gaiwvnkto.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gjqmkmral.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gmckfzpuj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gzchdnmpb.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gqipdzzhk.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gwrmhqrai.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/giuuxbpla.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gehnpxqxf.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gslfyxyup.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gmozvrvva.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gttkpopnd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gfxfcgaoe.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gulsgbwyy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gdfqwgbvq.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gcsiqbwhw.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gpgtjszzk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gziwunbxq.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gnfrudtzf.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gqkysgqvv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvgnsnsoq.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gktmbaqgx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gnbxsqagt.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gcksgcmaw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/ggpwtzcjf.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghsvqipmz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/ghgmlbvma.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gyxfkvhjy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gwxwddetv.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gmhxszjxv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gyumjfiwm.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/guckxucee.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggbbpjeuk.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/ghbykxvaa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gugoykmsn.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gixijuffm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gemdgzgns.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gmikzvhow.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gqxjzdhjv.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gkkgrxgvu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gxuuhxbfr.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ggcdlocux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gmtioiwti.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gstvjnorr.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gztpklaqk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gblguouqt.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gpawompfy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gboxjvfiz.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gacolbxqi.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gfkszmelw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/ggngdvmxx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gvlkwxfcq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gcxniximx.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gicrgdndi.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gokilvxno.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gtaucdvyg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/ggdsefmuh.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gbmnofmcq.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/girxaenfa.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gypsowrof.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gdbhdvenw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/ghfigfjfr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gkjespqbr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gxfillzrm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gvhexzhtv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/goxuytvnj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gvlvedrtu.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gaavxyfzn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gjnulkccw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gaurixaxq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gjiniglzp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gugmsjivn.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gtoydeuuw.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gorkadign.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gzrmouzic.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gplqpigoi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gkdnxalry.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gcwsppkga.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gvczgjavx.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/ganqujikz.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gfrgaxait.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gqmupgepu.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gzfmmrkou.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gxeftecnn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gdukiapec.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gwzodecpq.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gialufdny.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpzjseeuw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gkpewxaie.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ggsjfhrto.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gwdhlaiwx.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gkiwjwhji.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gxcvpzhgt.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gfnoyhfpi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gcejfqqba.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gxpgehyuj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gzmbhtvng.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gndpczajn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gerscrtnf.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gsoaqkkpz.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gpfwbafkm.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/grdltxtzs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gmotrawcq.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gnmoovpfr.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfpxbtccd.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/goigmxhau.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gieatoyyn.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gmdrmaavi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gnbarwlcr.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gppycpodk.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gsxznqtnw.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gtwrlqppc.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gggujneyz.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gflxnyfjm.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gdavukxgd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gaoptsksq.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gljhlwgqd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gopjjczml.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gdwtxvrov.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gtyleoslj.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gydqzykyk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gjqcqacnr.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gyiwptnlw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghqtedoyx.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/ghsunijpi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ghnvazmfi.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/giqpiqirv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gpscdhcht.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gbgeqnxzy.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/guznixcpm.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gobydadgm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/githgupys.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/ghowxopme.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gahgkipyi.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gmoedrboc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gjikjxspw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gnvtttvfk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gbiwrubyr.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gjkxlonkc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/guywxoarf.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gagpavqwe.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gbqctqsue.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gigiwdvyo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gtuorvhdg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gfeoafauv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/glcomwoqk.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gsnvukytp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gtpmvwkpi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqlgkushh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gvouxspyh.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/goecqfgze.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gxnrhjoni.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gubsjmjnk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/glaadtvgk.sHtML


<!-- 参考信息 -->