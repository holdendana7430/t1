代发 wailian999

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gwavjtlzo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gucwzdwon.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggdmojbrf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gaxnlzvsk.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/girzjrsqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggbbmuna.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gilheghtw.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwwvbcxsv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gyunhinqu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzagpzujh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleczxnhd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpdiumssx.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkkgrmel.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gznvmfzzj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gmufwlitk.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgjpcxrw.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gxraqnlme.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnwmxhkf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvurajdd.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaubfzton.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gqilcxpjy.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrkviyuz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gcgygivzx.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gcqmrhtmw.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsuinqox.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gyirqfmdl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdtqjhkfz.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlotetwj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/giddanmxq.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggofrmkab.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcgclnbxh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuhcrcel.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqapflxsv.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkjxvsola.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfnrjvmob.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/glltnszkz.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gyccrrhsf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstzxfbad.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gfohfpsng.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqgioqln.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gwngchulh.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqnzlsbkr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfthheiac.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gakowypfl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glsngfnqy.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfitxnjhk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbnepuca.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ginnffper.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxhdmfwd.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrndxnex.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlyepryc.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkskevsof.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giouukchk.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gykafixij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/guqrhopwx.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyhdstnz.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtvntkmb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyxlfmxu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcdaowvnj.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqjurdpy.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goobrozdx.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gmaznlxop.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnptspsle.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxllcmuet.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhhltzyd.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/guxsndxzm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gflfqqvsi.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gudshnhja.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwpeompcu.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwunhpup.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzszpmej.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqagbjqa.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqtjmtnt.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjiqldil.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdigsdrc.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmoypeqs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gbhbjkbdt.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghitdvsyh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdauhvhhq.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfkghmy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guzpbtfcs.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcaepqww.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveqekdkx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfceruwor.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaycdghj.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdhqrjji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gdejbkkzm.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gtdamactz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/guxryklbo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfvihlfkq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gtretzqtm.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmlxifpdd.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/godfeqgtq.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuzkkhwv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gydimkcxt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/glvdqqynh.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuoappfr.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvsltvub.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gihlbtops.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gatnyxfvx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrttdoqf.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvhdztcm.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtggdizrz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwezezknp.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/goxcfejjq.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gaveqxkjw.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gowqoalkm.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapqqpkgs.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqajvifk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gohjqofbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcyjthgb.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gikrkmdwf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gulhkhfct.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjfahils.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcctcsjv.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsaxfflz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywuawrjv.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrfyqncv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbyqxbrd.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/ghktjqwif.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmknolbu.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gvuokymxr.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwavaqma.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gipswedgu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/giifhfgaz.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnudruaal.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxvzilkwh.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gqnluwdmq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoablbbm.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxjanugq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/goswrvodk.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gpcpidtge.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqejmmmhm.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdobqoxgn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzhekfzs.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gjanqpxvv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gatlzubrd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbatjhow.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmkywthg.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsyljoea.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/groivkofk.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmbqdttba.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwabvlbp.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/ghyisvgis.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gpjavfxhg.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddwvdby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqumqedi.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gspcvhflp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gtztwcmwm.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvtzykksi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecybgaai.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gusqtqvno.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcfqmaai.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaotezqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsgeocyx.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gcjxuauyu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/glulovmjd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/glokybbjb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssfufahu.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/griavobso.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnylrjajz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlmptytm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmfkldqx.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtllpcgfx.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gyscxooma.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ggmsiausk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmbrlscjz.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfddasob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gupjbaynk.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvzjjtu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/guolwvskf.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gjstbuxpk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhlgpijk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofbtokdk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/givehvril.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gpreqotrd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqtmlayq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsvagvm.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gbtuocsen.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyluahrkf.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpvdpsbl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/givzhrlan.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzqqntzxk.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gdldrslyc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gynblatvo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gajiwqtqf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzxwzxjf.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkkyvcbt.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gahmctydd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkimswmx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gidwnwcdq.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkedkko.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gagnfrdzq.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmicowqok.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjnrorft.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsmmacvu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gukycywtp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gblvmelky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gddecgkcd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gptjrfxjv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gkcadeoks.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gedyuesuj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvjkacsq.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqsppfbzm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyvnbsra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpppnhps.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gpjudbftw.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxttnirdz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufmjnwmh.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gswfxodzn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzutmclv.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gwwhnepvk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/glbchdxqb.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiwmkpsf.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/giyzvhlbg.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gsibanwxa.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcvdkali.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gryeaaylv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnttqkmwe.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiryxjar.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gxzpwdnph.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtqvfbul.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoflnwqg.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gyusnnddc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/glxiazyoa.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfuzwtal.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/ghadrbiha.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdqpedfbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwnfqruz.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gfklceaic.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/glgfayzrf.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvuiqqwp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeriblsn.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyqkqpvb.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/grnmfeltz.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gkuvohsvq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllxdiqwv.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gxjslmztb.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghorxqiaz.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcybtrqyz.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqueuzsm.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzytyppn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghighhqcp.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gfweduzxz.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsnnliee.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbrxysti.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gsglfdosz.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuamsqft.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gnhzotugb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/guwbsjnqx.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gezdufnrd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gxjoqrzkv.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gwntbwmxx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/guemudopd.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/glnoleyte.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpfecrcy.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcdwdrwy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqunvidf.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gxubewwrj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqaeeaol.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gikdcaksu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkqfllwn.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gskhghaoe.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gegvpphvn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbvtroyuj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfijazx.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gofulkkao.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwyropjq.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gopjeacrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/grshylmdx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxzccuun.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/granjgdji.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gbfcuashq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gjholwmzi.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gfsfwhpkv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzlyhovui.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhjsykfc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvopvhmlr.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gnkqhkhzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gacljroxl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibzfwoyl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gywhlcudv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glggyuhca.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gvehaybjh.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzqmovur.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdicjgoeg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyfqghjf.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmlodgmfn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gicuzyvrl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrnxgzdw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfietkdw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsuhmxks.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnldkfbti.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtuonoct.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gbytlyawn.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdffbknjk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzhuagom.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gphaivwuq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gerrnlsre.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmaqmozu.sHtML


<!-- 参考信息 -->