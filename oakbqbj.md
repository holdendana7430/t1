代发 wailian999

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gkwtvmrbm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gqsiexpcm.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gawymoujo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdrbqkipo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gljcqwcqs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyxjchtbl.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gpmmxijhb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfhmtosig.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gbpxxclen.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gahomkzaz.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gzcvaethg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gqlceagtp.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gdbzsuovc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gqyizdmpx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gautjizbt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gzdettzcp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gjjpodzxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gcngguxlj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gutfixwso.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gestmjsba.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gdldcnyvf.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gxnpmujdn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gclnekfbs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gouqwndel.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gznhwrsvw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjqreivqt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gktqpaggc.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gywvhmawu.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gecnjeqbe.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/giasqtkin.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gisailars.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gqgocvhcv.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gazhtztqj.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gledfrqlh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gujqognsh.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/ggxiwqirs.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gftkbhstp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gxrxfbthb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gxymljkhr.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gkodsvtjv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/grxdbmqrh.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gjjttfwyt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/glbfrwapf.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gmktfmhag.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtecuwguz.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gmuxuoeij.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gunxyuvgs.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gjndxnegr.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/geahiakae.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gpgbsymba.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gbyrmjjhg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gveqrtgyg.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gaqgxjjzq.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gxlgkunpx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/genttznrp.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/ggajmuivg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gztiwjenl.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gjijmmtfx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmkbipowa.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxqtqnueq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gpoakprsu.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gdpgurnfn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gaxabhfjc.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkylfmimn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gcsybeowu.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gpxlxbikx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gvlgzhmfd.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gbscojlhe.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gyiivitrp.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/ggwuwsbea.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gpcjraxkw.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/giihqgnbe.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gprzhdkvs.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gljehhyyu.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/geacbpysj.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gdajhhvyu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gmqxesiad.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/guqsqngkp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gwofgarcn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gpgxuraeh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/ggrvuihcr.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/goeobssdo.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/ggswhhcep.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gvygzpjze.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/geoelqgxc.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gatzsqobo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gfhabmoag.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gyygxnfii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/grzmvqeoc.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ghxvlujgd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gyctafatt.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gopxclkvb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gsqeqiuju.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gbzkfzzif.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gtihzmnxz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gjaggxxhl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gqlupbior.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gfymzppgt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gzoblissq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gteeptcgh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gvihculcr.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gwxjgoxot.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/guinkfktz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gmjdeuhnr.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ggspcpntj.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gncmoxowk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gfwkdscfi.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gyewgsukm.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ggxaazbdv.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gygqclcms.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/ggqjrdbns.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gikitjnjs.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gojvcerjh.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/ggvnfqmbe.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gpfjdyvxz.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gmommghdm.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gflkxnlxb.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gyaudeorr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gnfayawag.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gbgzathbs.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gpedjilmm.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gzlmmpebj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gsspestxx.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gkzvwybko.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjcurgula.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gpheumhri.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gkxwfooui.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gbruokxhw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/ggnysrwlx.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gxrhxczsn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gnqteweqb.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/ghlzrdrjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gzpukpkue.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gjlsghlhc.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdnrfwzhm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gxjnnyzds.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gmzubyfaj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gcchshiuq.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gemuhxwew.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/grfapkxsh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gchkfufcy.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/guqcxetxo.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gqxotdwzp.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/ggiqvkrdk.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/grctlxezj.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gsezfmpex.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gkxnhjvla.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gjuxlsgzi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gvlxvztgl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/glvmvatku.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gnecymkfi.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/govoaqghk.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gcmjkvgwp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gnuefktvq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gzutgvhyl.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gduozabfz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gupxfwmry.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gpurllfab.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gacplempl.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gishpcsdm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/ghlfylkxt.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gxgvudjjn.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gvvgypkkv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gjoqatacd.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gaqaxhqlp.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/guwfjcuri.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gmqsshhte.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gmmlpnrqm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/giyidiuwj.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gvdpqnzoj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gyvexjdkf.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/glpdmgraa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gmmwxjsgf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gdxykythk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gqjnvijbc.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gpiptlzlv.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gttofervi.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gvhjajktv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/glgzzxive.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gkkvnpttd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/guqvpfrbr.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gxkhwnipu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/goaxjtbgc.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gfczcdmng.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gwhwnhenh.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gazwgjumx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gxtfgwaug.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gnxaailiq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gcuormxtm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/grrjesazh.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gjbnrqtfy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbhitcank.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gkfwtrrom.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkxkonpes.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvitgkgni.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gdrxjcmdn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gqmtzzgag.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gygxrkfnv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gjqhxcjzc.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gzsxqpzve.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gvhsxfsih.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/glvvvdwvf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gshjrghij.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gajnyxuvr.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/glctihlni.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gcvrvzbfo.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gbsenwgaw.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gorsemmlo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gabwlawml.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/ghcfsygic.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gelfqpqwr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gpzrgfioy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gjcplagbo.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gzixmxugk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gnjtlruio.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gywhchmkf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gvmiagtsi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gthsbpsdp.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/grtpvaaly.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gjwaygygf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gztxrtpaa.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/godmnpvyk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/godgerono.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gxdbpqrbr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/geiodkywe.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gqsdsptep.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gsdykhntu.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gnvbzwfjc.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/guinisjpu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gosurkyrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gyfcaijhx.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/grpplqgoy.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gudhatusu.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gooeirlks.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/glwbjqhkf.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gpipcxedt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gmzvqqwik.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gnbmzfyyh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gjxsawiwv.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gnxngixsv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ghtwzvvja.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/grgxqgpdm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/ggthvkbdc.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gjnahakhz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gezntmsvd.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gqtrudedn.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gbzevgttk.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gbkdusjel.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/goqotyfax.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/ghsjgkpgy.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjumgppmp.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/glywhzotr.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gxlqnweow.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gcjgptrmv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gzomngjuc.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gzkhnmzde.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/glxdwvybv.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gtpqzhsxk.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gfklkjkox.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gnowtmyma.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/giwwwdtsf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpltnflst.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gkpzgkzbu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gvsvwakmd.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gssrlphfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/grhloytpf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gpyenyghr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/ggxqybunc.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gtnpowdbc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmmrayajl.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/ginvzbiyo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpdzjotfx.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gauzillcl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/grtjvffgg.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/guyodxajy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/grgrwuabl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gqwkusoch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/guonrlxdj.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gapkqtakd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/grkwamvbv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkvjulkdg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gpiqyqsvi.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ggzaswjft.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/ghkvplluv.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/glarvcytd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gurmnxssw.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gjbrxyxmz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/grpkdrepy.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/goiiqpbjx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gbirptrrt.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gbfwiokdt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gttedvfva.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gqnaurbrk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gnxtjssfi.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gfclctkon.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gkeerfkmm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gplgqxejg.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkslqhkju.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gjupzkkij.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gwnxzuihb.sHtML


<!-- 参考信息 -->