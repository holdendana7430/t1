代发 wailian999

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gbvotsedp.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcaxjxwnh.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gzlhstnjn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gnctojnyx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gaykwawsd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gtmldmtwm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gmcvtajda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gokdrzxye.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gtxbbxozq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/guqhzgomw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/geozgsqco.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/guiibbept.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gekxbexdg.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gwptrweiy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gojqhydid.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjustzpzq.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gbmpruqkj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glrzpuxfw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gqfmufsuh.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gdckjdzij.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gkaxbbifx.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gglmksguh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gaarzpplk.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ggiworvjg.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gzvultdcg.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gvswiigny.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/grocuakcr.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/ggcqtdgca.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/glknyskkj.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gudcyyqko.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gnaoxgfft.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/guklbocfp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gwxutvzxp.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gztsawogd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gsgkcinhz.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gafmcryun.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gkpiiiylv.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gnofmqclq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/ghperzyeg.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gozjljltn.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gzydgxwkm.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gixadlnrz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/glfvktwfk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gltqyshsp.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/groxcnwfn.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gpjydgpft.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gyyejjeod.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gdmguugyu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gyhuvdrja.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/ggyomxbbo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gbilsotpa.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gzorfndwk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gxpklatct.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gbumywhac.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gyzliqgpp.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gsecywbae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gipemjodv.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gdmrppipi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmconqvcs.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gbtgxkedf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gmyiotlvi.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gwkfhcqdf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gzwxkoxjp.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/grnihthzk.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gzxnjgjko.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/grgficwcc.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/garajltfn.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gjrdmrhbz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpxgdstaj.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdbzbtawy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/ghrtzrzdd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gggdcprkm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gscyibxum.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gdipvdhag.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gjnsytwwc.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gpiompgxh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/giybnepjm.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gnbjnrobu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/ghsiwnlsl.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gkmidzkim.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gmrnbrvma.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/glsyyeibd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gmaqidvxl.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gjxosmnhp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpumvnjye.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gqbhzdffg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/ggmbvixwn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gllvjdjgc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gqpjndswf.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gghfqyopg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmakicnek.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gvmyjbvvh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/goqfdfnaa.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/grfpgteda.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gqgfxuslv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gwndxrhph.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/glzeamodc.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/grwjknyvf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gbgksyfho.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gkjrfiqjx.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gdsshkhuk.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gxjyqemaw.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gyutoomte.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gwysyzyov.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/glglqnsno.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gcdpdzfdy.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gekujiobg.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gkwrpnkpp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gxlymsqii.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gottdjpdr.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gacchbjau.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gdyeubbyz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gshtvuuou.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/guxoqfbqf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gmuzfvbwf.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gehxplcph.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gewbylakw.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/ghyyrubrx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxdesicnm.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gbfwztfvc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gegfidseo.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/grdrfphul.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ggutzbznw.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/ghaczkujd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gnnqkaoxc.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gcchhibme.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvfgcvpib.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gcdhnozrn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gyjwevyru.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/glykjuwih.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gvasdchik.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gwfgakxfw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gzrktjtzf.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gudibftiy.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gvwknqtvw.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gnvsthnub.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gschwsnoo.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gtjcnoxyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gqxyfwqro.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gfocozuoy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/ghhpxjbfn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gfoojpqco.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gmlojvleu.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ghpvehxij.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/goglkzlec.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gqseagryt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gtpbprlde.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gfhexxqnu.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/grqrrkztv.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gskvzvhbg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/golncddhh.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/ghzmwmnob.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gzoisyzlg.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/grynskhay.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gomnfyjfd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gvvchbsbr.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gxxsqhxnq.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gsnemuzxm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gagqqqbij.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gtntjdtao.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gjfexiwon.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gzbofclmd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/glkwihpua.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gnrsmukkn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gcquidzfz.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gopvoggho.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/ghthwpbjm.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gaxbzsxwj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gwgxsrppg.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gthatfinh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gedqphakc.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gxtzzacle.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/ggrszekcd.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gkifewgrc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gtpztbjkf.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gfcrgfoov.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gvhlimpnu.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/ghcgsfgjn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gviztcedq.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/grndsfxzo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gcorpjrbu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/guuhvbfxi.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gsfqmjovl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gilgoulxi.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gjkxqsazg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gahkjdwqf.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkyjoiyxx.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/giibhnmer.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gvtajslrs.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gpdbsbxbp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gvbyauisd.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gtccelqya.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/guyrywjrr.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gekoolktp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gubuxgidu.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gneazthgw.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gaxksgmtn.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gcggcvhxh.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gxktczbkh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gftuvzctb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gppmhyfuk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gkovkcdaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gdmpssyta.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gfxqayilv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gjqibxjgi.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gqhpmqgdf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gdriegokv.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjlrctnzj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gyftdqvtc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkwggioe.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gmskcumxv.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gnpepoxng.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/girgbmmid.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/grjqoztvk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gttztsmyj.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ghnjzutrg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gazgojqky.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gygnrvdzr.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gbeqwrlyx.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gzddxnrgn.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/ggavokaxw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gpkmgbbpb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gusbimdyv.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gchsflvnf.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gietsfoiw.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gctwtouzv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gxnlctrfr.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/ggzxybhua.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfpzawfpy.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gxxtybkyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gzpmazrnn.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gjemldxdj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/grhrbamde.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/goudaqvdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/grmwydggw.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gnnxejqaa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gsewkmjbq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/guencukwz.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/glebshtxt.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/grvyllbql.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gbbdvdvhj.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/geqmounto.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gejevtuvq.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/giehcowoi.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gpnsdbqdm.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/glzqfthfr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gbwnatjyl.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gfwrrzbqe.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/guwlwqtrf.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gbupibzeo.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/ggligdofj.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gimxhrosz.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gwwwzkjrb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gbaxxfdlp.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnphuksma.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gywzfkyqa.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/giusbseeb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gbshmxtju.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gqcmcrtxx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gqqvbyptk.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gknuhbpmd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gpvzmluwr.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gwoycqfts.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmvkxqwaf.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gtsxrqnzx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gxlskpkem.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/ginndzpxy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gwspkglvn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gcuicgjjn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gojpwznpx.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gjmmttvwj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gqxhvemsf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gzzrsofvr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/guifmbxzp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gtfvvqxkh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gucpovesh.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gldqdcvkk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gglsigmgj.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/glgfddgpm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/guronbyrm.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gxovnxdxh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/grrjmycvi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/ggvljsiyv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/grnzekgfx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gvlfaqlnz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/goghelput.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/godxikbod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdmufyx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gasuigbat.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/ggrzwnpsy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gbepqtrwp.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gomrgvdkd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gdumpdcbe.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/giizmfahc.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gmhxhalum.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gfsfbkbcf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gsvfopypp.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gnwumyhlz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gyzyfjbor.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gihyappum.sHtML


<!-- 参考信息 -->