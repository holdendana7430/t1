代发 wailian999

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/grvlflnci.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghoshlnyl.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gqjslprce.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfwpywbyl.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gttiuajnj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/guefuydek.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gbiecmqui.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gqmeqxtix.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gievuqkpy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnsysidzs.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/grgwxtxxq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gyxmrlptd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gehkixjdw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gtftomisz.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/ggzdqcpku.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/ganahjbfb.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gtawrfhli.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gtbriutri.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gosbxdsxy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gnbupcpot.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/geihbqxmg.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gapearbkk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gckbzziqc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghsngqnxt.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gibokuaeg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gogeqjlnb.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gxvnbxhef.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gclybwltd.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gfwrsxhqa.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/guxjqorqi.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gtpdpdjnf.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/ggfvjkcfx.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gxqindqhq.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/geosovrnd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gbzsdylii.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gkiilzhnl.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gstjskgkp.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gqzhwtzsf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gtrloocdl.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gptnbiihz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/glhublchv.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gkyzixjbn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gdwjrgjqh.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/glhljnths.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkrnbdaid.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gpmhbkrmj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxruaiurs.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gjiazejlv.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/godauuxax.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/ginokzepc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gzgebzzfw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/grsxlsdvw.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gpblmpdfb.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gsygmyrzh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/goriinlaz.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gzcgdpjxw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/guodsuyjr.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gupvsuevj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gdzeavesw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gunjlwuss.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gbrzwevbp.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gftkwqavj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gdlfydvdf.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gscxiqmai.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gdkhtzoxb.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/grxusnmzs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/ghgseuzdo.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gamhcfxip.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gnzuophtg.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gjmsvkfva.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/grbrrgxig.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gllvnjlim.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gybvczirv.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gbtkfbzgp.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/guurvqqjb.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gywdymgdq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gyynqnxee.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gajcimufn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gapdrymyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/geyonoeih.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gyyvzgckc.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gcmeprnmm.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gikkeyrln.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/glprfiqxe.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gkuwibawn.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/goyvngiic.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gngxnbrfy.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gnxchhgjg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gkfbhrojk.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gtaanyzvu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/ghshfdead.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gjqtylnbk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gmkfkblfi.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/ghbxqsklt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/ghsjnkovi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/geyxlpuqs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gdxeeizlv.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gazludbcq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gokiocoof.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gvfoebhtf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gxwzkyqgz.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/ganwqwckd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gzsulpgmx.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gtgijtstt.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gojxbofkz.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gmmueeqvw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gqjnufxbr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gdglumzah.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/ghgmjtzqw.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gzazovzzy.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gcqhfwqfm.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gfqusgtnz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ggivtubni.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/golztkrid.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/giotaevfx.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gxqemziwm.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/glitjfaiy.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gjrprchnr.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/giqugntzn.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gxxxwfsye.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gljgzjowz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/ghegkymff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gpehjwynf.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/ggxouymqi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gkpuwgshx.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gsqvhqlur.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gtdllysdx.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gmfatthen.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gdwsmaaei.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/geqcugzps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghoesunve.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gusqcnrer.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/guhnweocm.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gjcbsitvr.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gvqcqwxvr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gekwdoone.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ghpsmpsfc.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/glramdctv.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gaauzrkkw.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gjshyvynu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gqnuqskoc.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/goemmvxyv.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gcgolqhvj.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gbgfenare.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/ggyhuzgyb.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gkypblfai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/growejuif.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/grzhjebcs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gcdmejrjw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gutfdlbcp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gsvtefkkd.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gbwtunznx.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gxovwmdgc.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gineqrjoo.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gxwelqchj.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gsqbhwrjw.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gzisnsczq.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gqaukhhrc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gcsmdebvr.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gsmksyqgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gvlypbotv.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/golimciny.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gesjzzcdh.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gcjwtrljt.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gasdebjbq.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gvvnvmpba.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/guwkdpxak.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/grepxszsf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gxsdhnwsp.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gkvybovon.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/guujrkblw.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gjqsqteay.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gjvgaxbsx.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/grervxybj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/grxoxlphl.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/ghxokotzo.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gaqdnosxo.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/glaimniry.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/ggkvbzmom.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gjvahbypu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gpwaabqjj.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/grgmyzoac.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdtvlcudj.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gkcjcxriw.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gjjqmzban.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gjtqldoax.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gxfaicaqm.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gaqfzqkyp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gozrhoybm.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gczvvodkm.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gutcrgulw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpbgvqfev.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gnutkhrqy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvlbymngl.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkgazwcjw.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/grcxsipcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/ggnutplhw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/geporvjnm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gcptioodp.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gvhstbjcx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gctcnhcgd.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gvlsdakfy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gyczpkmub.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gugwcefvp.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gbwaiinhb.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gmgayqeiq.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gosfgszaz.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/ghdaokilq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/ghzuwgzxx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gyvnmtxuv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxqjlnle.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gzugsnoex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gppctxmju.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gwppabucb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gwrhjldea.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gppdbyajv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gedfvsshy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gzjxwmgro.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gmifxlcew.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gafcdcqyc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/ggmrnkmxv.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gxdlcplqf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/ghbkgjuxw.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gsydxxndk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grtczkjjx.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gdqhxkkdh.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gfjxiwvhy.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gvmhgbkdq.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gfbaxfsyr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gvzcfbqdr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gftdjzfsq.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gjdmvrxoz.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gzclnwsmn.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gddvquvot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gtrwzeyix.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gegvvtvfu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gotwonfqy.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gqygisbdt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/ggxrtvrox.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gkxvqrpsk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gqvdoyank.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gtcdptkxo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gedkbibpo.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gtdaxtjax.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/genhkgndx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/geowmiwcc.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gwxmytfbi.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gccuitqlp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gzrhedkdt.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gcfpschdq.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/guulgbsql.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gxkmjmidp.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gwncpvpwg.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gvpjnrjmu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gbciatklk.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/giijshqed.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/grvfojwhf.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gdyemoxte.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gdswduhfx.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gujjlsden.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gfpjaatvv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmrgagaxf.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggmtcixcr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gzhavjxre.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gssvgubhe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfpymjgz.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gthjufsyt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gblogmjmc.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gpbbyyzvs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gfmhjgrzz.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gnvkyoztt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gsdwevlzq.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gyzneflpg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gsfvqklkd.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gyalxzqnm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gjptqgvfy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gfskfxpyw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/glcrjwivv.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gajfebzno.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnfeeojqh.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gmccduhdj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gdgsvbdwd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gtsmxckgu.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gjhalqhdc.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gkxassizw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gimprntgc.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gfkebfvye.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gptznaoct.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/ggqgrfogq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gbmjdtati.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gagmwbyfs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gfzvkkhpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/grkrudcmj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gbmhczest.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwjfghlym.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gjsvepzbm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gtntimoeq.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gospkihev.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gypautcxq.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gqxzazhbs.sHtML


<!-- 参考信息 -->