代发 wailian999

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgyptseg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlqwqjsu.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gsceqroir.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkfckbpl.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/guzvjerzx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/giwxfrbei.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcitbjkdd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsblaubox.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoxfjjpv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gubgarkmw.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gshohnoxw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyxkmosp.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gxodimeap.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlmvaagu.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gjudyebgg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gnaetuvuw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcifrtmi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwbyjal.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgmizchi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmoxlcff.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glescjlzg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdntclkks.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfibizgpz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrwtynd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/grcawveyi.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gnxsomreg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gposlqwkv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glmctucen.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/govfmrswr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhyypmwh.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gfzdcmbou.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gtshrbeup.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxilkgxw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqudwurf.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gslrevlfh.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geetujhqr.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gsnptmwtd.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqullspjr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/guhipbhuz.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyugmbpga.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gomldnpta.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflazyqxu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gipctlend.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guanwesbr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gybhajnxy.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gslsdrjde.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghxqbwizs.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjbxgzpk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gisufbmig.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsfbdgbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqcxviobq.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvmzlsuk.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqioxen.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvupcgvi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhcbkmea.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewblfyjb.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gfakjlogu.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtgwrqoon.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gytvqapwd.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gremyzcrz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtijlixfr.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gvhhnuvco.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmwkiywud.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqykcdlc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggabqigvz.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghvfzrinc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glnrrfgeg.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrghiex.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjruplbt.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbnehioq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdtvimaim.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlfaxqjb.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjvmqhyyv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmlqwmcw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcacprxzj.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmlucmc.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaaoobes.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/govhywvib.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/grssoenye.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzldojbmv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gihlgbylw.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/giwqdmqfk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gazepdbte.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/ggcfghgqt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gudlchupq.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcvgrgwgl.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gjhsuyyem.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/ggpzymvtx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gltqdagis.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigychep.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gjoutlrne.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqhrskhux.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgetvzom.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gsmgoboul.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gofblqkrt.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnnomkljk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbmeohhf.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbgcbfxz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxltqxhl.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gotflabow.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfrgoird.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gzfpqhsvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhmjdojm.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufjzdrbf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gzomdkllm.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gpkeprkcv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkhvxnhm.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsajbadti.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjakxbofm.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdevneglg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbmgnppz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/geouwwnec.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/galqmuanw.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzvzitzd.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/grcfifvqu.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbkhzyoj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwhrwook.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdrzzkzu.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/goustkthi.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gekjcdzvh.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gtogtegni.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbbrjjpp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvszzwyd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gbhpmarqj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gmbwwvasf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtssxxgy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gxqlfstfh.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgjcoxtg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtucocbfi.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/giwgzvkbi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzfubixi.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/geplctegq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssoksjji.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaeidbqy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaurdbpy.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzuxnpqy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gecghtstd.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrwhryku.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gprmqklqa.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvknidpv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glfjrhvsf.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gclpflngz.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaskqbga.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gsuuiorfi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfprzciid.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghzvumgud.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ggxacqnyo.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemtnuws.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhgatddn.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxgjlkcdr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjgxctrm.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gewkhdksi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvqiuvbom.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/goilqzeth.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdpsoteq.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gggusoubh.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gngzphbrp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gftontyfj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gqewsrhhc.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyhzdmoj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gqbmrljac.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbmpkikx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxlnidyq.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeqwuehe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/grlzquyga.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkppmvkkn.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqcebpjp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbwkawnx.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gtobiexsm.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggudepdpr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtucpmtzw.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdymbsuqo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/ghcrutcjp.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/grmvalxag.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gweuebhlv.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gprahoagv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcczxvpha.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gffasdsxu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gttoeazvd.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/godvszdxe.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gvyskszko.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykpzawiq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjharinbq.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grogvulyz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gshzedfvk.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyipkmlv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqltdnnsy.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpoukdsu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginxjgnak.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gevsljejl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdrnvnzd.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gooskrcpe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/geqefukgw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujqnvezs.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfdbusyg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqjervkc.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnswiogwn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcxamkvuz.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmpbpotus.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggehzothq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbwnoser.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gcdarhdff.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gshpjrygb.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpkfmlqp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsimhjwq.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvouaxscr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gccnwohbr.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gfgrlrljb.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcgchzyjs.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gctktgppo.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/ghprzcupw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdhvxpxz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gtzjyvjpz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gdttsfbla.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/glbvgbqyy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwegmqlpt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gtgyljblr.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjrspfaf.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqjpvtkz.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gidwgnxlj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjejfcaas.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/grtxdxrwx.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvuygbddg.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjsjyuuxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrhwtrwv.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsxhiovw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gprxwdtjg.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcynjegl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/ggqudtkmn.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaqfbjfb.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabxivttw.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gffplkokk.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjkyjjyee.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcwyranqz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlegdiev.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoicdfmh.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gqjpnbixn.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqostupyy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdpwrvyv.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gwamnthzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grcthpdya.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gnpblriwf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbfvaeog.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvihbevy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxktkkdc.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxkezlxg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcflbcsvk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gaspxhzzr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gutizxjaq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxgcpzlu.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gmtbvgalf.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gsbtpnvnx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbxtiiew.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gfgkksfgj.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyddynelm.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsodflvc.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gdzsbrvqr.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grgosbmah.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gmzqiggzm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwgazpcr.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gfswtvens.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gnljddfvu.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gdybkazzg.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grrgolonr.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gibnkguxd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujhwrre.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gohkutvpx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpiubzmad.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/ghvcrjphn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfzbdcjy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuhcglwm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaopfgufk.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gowwdzdkf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicvwiure.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcljmnku.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfxbizx.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlmzntsw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqqeqxjz.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gumtkhclh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gshlwnevz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqkyvdri.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpgavlgm.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghpvfenvl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gueunivfz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gimkolupp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyazhtwh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvrwjpbk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/guhyuuhde.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gdclokxxa.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/golkvbzij.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gzjfyjhga.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbuogwsr.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/goibiaulm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpstqjvsp.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsfifcyg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqlolood.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqjpbkjjc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfwwtrscs.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrnvkkxi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gzfpxsqkv.sHtML


<!-- 参考信息 -->