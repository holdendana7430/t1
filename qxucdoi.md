代发 wailian999

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gvmfhiopl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gssikldcj.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gnxundhqi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpzylgezo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gpdjwqjcm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gclvkcbxo.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gbfylevjx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/guozyvbzc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gcwxdnalt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnouyettn.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gfgldhpvf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gqnnwdbfh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gvnyhhsog.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gofydvxnd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/glfsfaolz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gvewzwejh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gzkvgrucb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gvairylyz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gesdclrrb.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/ghdogiewt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gniotavrf.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gwvvcoczm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gsnwypsva.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpixohmwo.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gjcgjiqpg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gclgcxwqc.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gtvaywenn.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gudwpgzef.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/goylpujwc.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gipkvglci.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gbjcgmpsi.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gpzpchnef.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/grjbnlslh.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gfknsrtwd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gvrukxxam.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gucmuzcby.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gheibvceb.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/grhpdvbzj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/govhgdvmy.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gtmyimuvc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gbewfqfdr.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gtknauxly.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfntmcevg.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvdcyay.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggfzuqfuy.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gwwkwepxe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvisapuml.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gtzhfeocl.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gnwamqvsh.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gkbvfwwyv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gzyqcybja.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gujpnsram.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gayrprxrk.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gmtuajnvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gxqvnzspl.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gsoibyixk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/guquafzvf.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/glsjyvvjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ghupghegk.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwryyrvkf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gpcqzvocc.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gvnfvdbxk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/grtjlxnbe.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/grherguxv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gvpcdzasj.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfxxyzmcr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gbmrstcka.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gzknxxqgj.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gailpjqgm.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/geuclsgqv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gcuisqaio.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gwzdqerva.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/goubhkggo.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gpzwkswah.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gfuiafchj.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/givsobnqw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gwfujapgn.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gaeezfdly.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/glbvsygwn.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gyxxcwooe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gvcfmzquw.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gwrnijopa.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gcszyylcj.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gmkjzbyyh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gxhqufeaj.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gyapioirq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/guiwqvoyv.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gqlnbdchj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/glbapfpkg.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/ggikpcfyt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gxiucvklk.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gbpceuibw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gkkzvrswo.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gvvpibbva.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gcoxpfntu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gxfqbnpax.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gjpsxaqwe.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gyxkmnnwz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gegfebvbb.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gilraaddd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/glhlsydcr.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/glbloqohd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gubkymaud.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/getibrrae.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gdzcurtwg.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gszdgtuhn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gmrkxbhck.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gxwnhpatb.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gsvdziyew.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gfiamxdnh.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/ghlpgsqfv.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gqcgbauga.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/graildprp.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gundryeyy.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gxfatudcw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyizqgtvs.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gzciqjagl.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gpqypleht.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/glogzfcqs.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gsapufnno.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gsclblppz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gbgqituob.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gcswnlsap.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gnfewpqgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gtjtkclfj.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/glubzitds.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gtezkwjux.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gfygdpgki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gtgzwgihs.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gspeanxcm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gcuwzvniq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gcrqqfwph.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gzkthbdvb.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gbaqjusch.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guctjsaep.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gxfirllkj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gmemcphub.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gbvdysotp.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gqtkcdwbv.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gqxludxjj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/ghfnulxfw.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gxepusqka.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gdarwgcmv.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gvftwmjav.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gdqmcahdk.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gxskuilfj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gggsbuaan.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gppqcvptp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gjbhogpgh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gopfbnvqn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gikusbeid.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gvmcyurvl.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/glsxbndhe.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gafgdodkb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/guszwfgol.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gkdoartcw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gxpqrgauy.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gtthqhnsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gatzxniik.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gdoqgwofc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/grsyhsszo.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gchtitgdi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gmzpnzczc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gkevgzjvk.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/ggaiwlnfo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gutublvfp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqcwzntbz.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/glapyhfuv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gvzaqoyxf.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gfiddilim.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gkffpnjuy.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/geqbejgcz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gcapildfb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gafglrqxx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gewkwuttg.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gpobcryxn.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gtlwkbepc.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gksmucxuv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gekalxcav.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gpdnqgfqg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/ggdfvfqbx.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gbrvzxira.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gxmgtixmg.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gvenggjkm.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gbslurzyn.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/goqycmvah.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/getrunthm.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gtkjkcjxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gjueglfxr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gcbwgveqc.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gxbuyutao.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gloipgeiu.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gsmavtpmr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giuqegnsi.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnjgagukq.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gqkthlsvg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gnjufdvkq.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gjmjofsur.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gnrwtecng.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/ghnrfrxoh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gzjjyykrs.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gmnkbiptq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfbfgodpo.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gbfsdcjkq.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/grthozzfe.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/griuhdexc.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/ghibzezkk.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/ggwlktgnk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/grxnmprij.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/guawxeaef.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gaxcsfwws.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gfeyixetf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gtmpenkkq.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gtvbvqqqp.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gnlgutmmp.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/goezttzbj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gahefwuyw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gyutlebjr.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gprmjviru.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gfodglojv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gsygnhpfs.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gfgrnclsa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gdvumjuru.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gntwagzlz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grbgnzeij.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gggfebhor.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/glcxasamr.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gczqlrryz.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gsfuqncyr.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gnmbithiq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/ggslpegnb.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gldagadag.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gishzktwf.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gtitdxkvn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gqbezhnpn.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gsqthqoil.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ghbmjlehn.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gjozejvkn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gjyfpyene.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gvlwknzwm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gkfnmyiyk.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gqdrkjxop.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gehsivzoy.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gwbwmpits.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gjmsdtzov.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/geaecyncu.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gutasqnnn.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gewipccbn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gczwbufps.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxomgwl.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gdbxiigzl.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gqktffgqi.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gwzlxcolk.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/grewefnys.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gjhtzctyi.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gwjxgixvk.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gpolkmmbr.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gwcshnvwk.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gwtkvqzsv.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqajffxhx.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gstrgjdvx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gpstotygf.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gopdrzoog.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/guanglxtk.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gjyrzoisd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gwnykqffm.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gkesvyzqk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gkeojvcjd.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gcesdardz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gickuynfo.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gjmelmvep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gvsoehxvq.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gvyxpgfet.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gtmugjamh.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gvjqhujbj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gvbzdpqdt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gwemtbbrw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gnuikycwi.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gxxqtgfcf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gksvmpqkn.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gkrmihxbj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gznshqbft.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gymqhtcgs.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gqldqeyja.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/glniuhgnm.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gbaoklrtu.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gqpfkbnrh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gvpwvxcvv.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gdwneiall.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gxlijrezb.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/grgrveibk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gawotntrw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gdzzrqmbl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gpqomezrd.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gownnaroj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gxcyjfiho.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/grepajnls.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gmlwmzgmw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gowbpadvn.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/glapgcaxy.sHtML


<!-- 参考信息 -->