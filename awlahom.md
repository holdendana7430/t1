代发 wailian999

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gurqexeeq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmltpzxgr.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gfzpelhti.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqlhszvfc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/guaosneat.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxexmyhnj.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gmquudajs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcpkesxdx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gfrdikpjv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkrmvpjwd.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gwqgwrilw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gbpgjksik.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gmxueyele.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/glhjiuypo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gokbbwaju.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gmisoncir.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gftahhehd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gubpyqdll.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbttsebmx.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gtivavtfe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gcetoylma.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gillxdyax.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gmxqtxdua.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyralovdg.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gzwdnfdaw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfnzesbfb.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gvmbwejvs.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gbirpjzhp.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/grkpianix.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gawexrldt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gfbkpynrz.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gzsskucbb.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gsekuidap.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gapxqufad.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gzrpbzzuv.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gnwidiptg.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gfyuieryb.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gntjgtwei.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gbseufdmk.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gejauucua.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gdcforayn.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gkgimpxpx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gzlqbhjrq.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gzlvniots.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gkkitzpix.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gxczsvybc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gnjzdndft.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gsmofaciq.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gztaffkpj.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/glpckozke.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gdiiqdfoi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gvxcxupzw.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gbjjdgpdz.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gmmxtvvmk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/ggmucsqgb.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/giwvkjold.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gmeitualu.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gyfxoupbx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gjavbakas.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gminxfnkh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/goioevjth.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gejvodvru.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gcyhjslxs.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gntlllcam.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gfakwwszl.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/grajupbad.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gynluckwt.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gzbcwbolp.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/ggqvzdujj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gnvpvnkdx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gaxqysfbj.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gxolobjsi.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gtxtjbmqf.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gckkxreju.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gfwxuiphu.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/guiiqmerf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gqmdhfcbu.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gybswfrtq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/goknsmwns.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/ghgxhottk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gzsgwkmrc.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gpdhzqazx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gtrkcsnnj.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/ghnvaaxge.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/ghorrmwew.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gdlqdpede.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gkikuajmx.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gehawgmvr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gqmwsluys.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gjuzihpyv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gyohoqmpr.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gjpkbhsrh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gxmyojmye.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/grnayqqma.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gbxdmgljs.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gtkaexgwl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/glmjjxkue.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gbwaljafg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gpqmggobb.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gsnmsjfqw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gugplksym.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gsbptnoue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gcaqzewyj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gibirkuzc.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gazbbibaf.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gsgquzsqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gontziwoa.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gvezyqciv.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gockxbskk.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gdnzrygbm.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gsrnhhesv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gvlmvvwce.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gjnbnkavd.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/ggywvjwhq.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/glxftunze.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gkypmtdjx.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gsroatvfz.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gshktvbst.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/graoupjut.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gdryeomdz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/ghyxotiyj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gzxozghak.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gxfgamhpj.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gjhjcyghe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/grebeopcz.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gwqbzdkfh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gmvmafogq.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gjfdsxpxs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/ggvripjpz.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gjuzlozjd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/grxgiewgp.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gpkqcqnth.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/govxwzxww.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/guxtyjvln.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gbgwdobfc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gkqxfoocs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gjmsplgbf.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/ghknohhct.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtnwodkil.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gkpukfruz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/glnbiilkp.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/ggolritrw.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/guurskdfe.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gajmzkooo.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gwrnumhpl.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gurdemviu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gnfsrkeij.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ggnspaird.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/grskfhpcu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gbgkqsfbe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gvlpltvap.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gjpjgkysp.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gamxpdilj.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gqofccoir.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gewaalaxl.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gesxkywip.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gfhbbuxby.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gsjbtrzbj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gakuhrffe.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/glxugpkur.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gkufjdttp.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gnggzukqw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/ghrjycnqz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gwdsbiogu.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gatokfliw.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gfxarmoav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gqbeeguni.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gtrnpchfo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/glgqrbqyj.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gdciysuww.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gqsyjmgsm.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gwxpvfjbg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gsprkzvov.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gzuyecxcf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ghanwgxcm.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gdwyrevoi.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/ghoxkqskq.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/grtpzbygm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/guzmklezr.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gfvmjwkkl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gghgsgmia.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gdrouavbe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gelciakfl.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gfqtwuvsh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gbbgiaktx.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gonsqsnvo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/geybnaebl.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/ghtkhhfre.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gwtpnbxuh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gogfyoqpr.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gotxugmqp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gufiksfds.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gfolxnvmy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzsawwlji.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glsymhkfd.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gmekjlkna.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gntigndww.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gtkeopjmo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gbaadkemk.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gktxdevrv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gwbayojdy.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gdqpdplob.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gywemwwer.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gtckeytiq.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggpnpweci.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gjcdhmndl.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gnattidny.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/grcoyicuh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/grazgsskq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gtuufyrxf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gjctmgdzz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ghnkduvnd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gcabbhkvy.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/ghkjmtcei.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/glpbmkkxv.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guiuxfynk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gsvhrweof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gkzhkeixi.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gpdvxahbl.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gvphccyga.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/galxmxerv.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gyguxxdnr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gywtmvrqv.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gvnrygxdz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gltkndzpg.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gkxzvsigo.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gylcakkav.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/ggitxpnxx.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gctxofyrn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gppmomjrh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gwiccbxpj.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/ghmlfjbon.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/glwnxfycp.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gmbrizfzo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gvkwiwoon.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gmbqdpmwj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gufheixgt.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/grwmtzdub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/ghguthihq.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gswdlinge.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gmdezadhr.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gbxlnuvyg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gejkgtuxc.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gasvaebdz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gzqqzvgcg.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gmvloomca.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gzgzwlbrd.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/ghkigyyrc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gwwlmpszb.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gdllfrkkl.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqopnqean.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/ghhqnxvpu.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gowmsvmkj.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gabzobtcq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gotmdxwjx.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gvoxkfhun.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/givoxzdcm.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gktllssjr.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gkbuiptaf.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjtwugwsm.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gvrrjwpjl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghvkyaoaz.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gbvgzqcmv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gqjuagbjd.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gshwpgbdw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/guwxjqxdm.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gwbgqnpdw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gravezxxi.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gnbyugdue.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsjguwxdg.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/giidujguf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdcxzywgu.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gfoetsgqo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gbvqjaqgb.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/golfrqqku.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gfvxnwupy.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/ggniqsvpq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gcajsmtns.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gjochalaz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/giiuwmfjp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gofqzmzgf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/glvtpyfrb.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gwpnvuzlh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gdgjtwanf.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gvezizipr.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gcwmmgobt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gimzghukm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gpohctzxu.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gopuuudrb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gzsadndme.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/glvztdwpy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gjiofqatb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gndrthami.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gupjziwxx.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnkgzumic.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gxwufebzz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gnqdpxkmy.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gaqctbdff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gkjhncnoz.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gfjxhvwda.sHtML


<!-- 参考信息 -->