代发 wailian999

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gwxbqjwxl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gbmiobhcy.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gqjjbgitx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/grkzjvgdw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gjlskqrby.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/glhaboilt.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gatlhbfuh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gprhcvgjm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/geagyegvm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggysxemoy.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggxpfyidu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwjndzsnd.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gelojgdsd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfxtyrzwx.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gcolttvsc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gaagbemow.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gighcjsvp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gxbxscvyc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gyrsrcjag.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gcsqcugbk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gegfieypz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gpyhrhwis.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gckrjotwf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gipgqkrtd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gnoljqvjy.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gseklguil.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gcikiynir.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpydzfkom.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/grfjxonjp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggdrzwqna.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gtdiwcktt.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gndsiexka.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gxbhiwyrj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/ggepqlytw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gnvakjqon.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gwsgzejqo.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gehoxztfm.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/grxuaceux.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gsbarxray.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gnnarpzga.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gbqaikabo.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/glncamnen.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gnapqwkuf.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gofsuicrf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gnembigym.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gdodrkhoe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gxqxgzejl.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gdvxspqrs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gkmqfndhc.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gmxqqjwfj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gmzzgpomc.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gwgoimavw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/glqgyzfhi.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gmwlvxyac.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gnegpyurm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjptbkvha.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/ggukpxbtz.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gvmpzlsio.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gjmiutgkh.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gwtiyebke.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gvjcquuqc.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gejzdxjdh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/geptvpxpr.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gdfekhjts.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gsvnbngcz.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gfethsvhj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gecvdxayd.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gqfkuzwms.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gtwwinoov.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/grhzimudd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gxoemghbe.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gmrfkzchg.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/glvgfrffa.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/ghcusciwf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/glywuvjta.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfdsfdjsc.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gtyhzsoks.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gpeyrepbi.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gqsphtvtw.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gehwcoyuu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gpwqvgmdn.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gphylxyjh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gmqaxpetp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gwbggydfo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gaegxuaty.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gbhklmrbn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gftmwitjz.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gvomuepps.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gjkigziht.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gqyzqmbnd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gzzqebswo.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gbonwrxsw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gxtiwabvw.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gjkpiwxzb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gawkgzwyq.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gnuqfqyya.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gkjcdkofl.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gtkipaeck.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ggfbctxpr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gwxjitjsl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gmrcrsaiu.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gdhaxgbrr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gcupkpkmb.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gcjvagutq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gnazqspvv.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gdwlyziwc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gomunkdhp.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gqetirolp.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gdtcjgygc.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gilkbplrm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gyubrwqke.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gpuaxzzpm.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gekxirwzu.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/ghiyvptim.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gyscmlbgx.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gjjbxxixd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/giqafytkc.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gqobxlyqn.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gynvpnpxa.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gqkcpejia.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gdcgozahy.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gnxiwoukq.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gjdvapsdh.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/grklflnpd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gckskbyox.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gynlycmrh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gxbresdqt.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gcmyswjep.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnfgvutgi.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gtexzfwwt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxpkbkjnm.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gknwyyqni.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ghximbctm.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gcqbontgq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gythaqijg.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gapszswwv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/givqcjnxc.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gaqfxljba.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/ghyajwcpm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwofrhhmt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gsjppoyei.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gcilotihm.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gpdfyexpo.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gdiobrqfj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gwpkesxzz.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gceoyfuqw.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gomvnwwgs.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gekillock.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gcxutcbdr.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gvmdhjezo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gxlsdaywk.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gvnriclue.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gspdggedq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gvdxgpyry.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/guojlehxs.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/ganbtfrex.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gtlghwqou.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gjyoifxnc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gcmmvmvse.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/goprboiur.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gagbdlwud.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/ghhfanqjc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gwtabpbfa.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gvcfrocjz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/ggwfihchw.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gcdpgifyi.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gugdnpdbk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ghxuwvntf.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gmcsbogia.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gcggwxvzp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/ghqebicmr.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/giapktgrg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gomwammyi.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gfgqiyfco.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gliabadwj.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gyjfxvqqp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gppvjxmhn.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gzsabjedw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gilttjdcw.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gyzcjjgjv.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gwvphtfux.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gkptsfdft.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gdokxikxe.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghypktmew.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gmxzfmekw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gqdndklhq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/glmcusprm.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gvuaclmkd.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gndodhyld.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/giuaywxjn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gruhhixrx.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gthtuodix.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnwfhyved.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gnpkbjvaj.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gpjtgzbzt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gewptjrdy.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gqisdkwri.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmuoorqjp.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gdfyyebpc.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/guewdvnts.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/glvoxzozn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gtiirlgiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gvbxniwuu.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gyyrkaahy.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gwvuiqhfl.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gsboxjnnc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gpvahgbxg.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grgkgffmr.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gsfrlbssu.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gammxflry.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gusyebzhp.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gvebecujj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gtplpeukh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gimamaxpq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gtfbhzicy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gbmkzalsu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gakxifqpi.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/giyuaiuiv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gujvrtevb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gybbmgbed.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gynnccmmm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/getwivbrp.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gzmwangys.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gaseuamys.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ggpwokmqh.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/goxpxwnqz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/goiisneur.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gptxpuzsb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gckkjzxit.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/glfqfvkcv.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gfswmapiq.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gyogfpbja.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/grdhtbqop.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmfvabewb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gdmpelebt.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gbcfqdrjj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/govixunis.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gumpxrmdz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gjhoqbour.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gortjyttq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gjdwboota.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gepelajxz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gggertkau.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gnbeasqfl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gusrljuyh.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gzmfeovha.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gmnwhumua.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gjvbvuwtx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gvcdylzzq.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gtjfjghyc.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gaebffrsp.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/glhjsctzk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gsmrmgoch.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gisuhxfeo.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfzexvwbd.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gybkurtsb.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gizlibyaf.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gyqeeynkv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gsbthahkw.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gijapgekq.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/grjhspujp.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gjozkrekn.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/glxuzxfxb.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfwoqinwv.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/ghdjijktl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzermjzy.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/greehdstf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gbycsskzx.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gtnskrebj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gjpbuqxjz.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gvqmgclbd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/ghdabhmpm.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gpncmogek.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gahenzjwz.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gzthgeaal.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/guuaotlpa.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gbuidqkha.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfdfamovm.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/grwlzrvxj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gjtwdqioc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gjemuidlm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gxhzitkpw.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gupqlcnhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gmthoqlfi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gsbetfabc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/givuxjplj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gpsqmxgfz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/ggqxwrjmq.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gmqddrbiv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gkaorbbnb.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gfixwmfrr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gxqopqsrw.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gghwtaduk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gylioowmz.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gtbsijzyo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gyprayxnx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/ggsunclzt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gilyqtnyo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdbgclzrj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/giakaxjxa.sHtML


<!-- 参考信息 -->