代发 wailian999

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gsypvphcg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkcyedipn.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gujbxmyqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/goyplgnec.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gkeqeqsab.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gdotyoszp.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gbopcgtms.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gssjomrmw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gawxabwrl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gsbwdabyp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gqvwffwyr.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gjszxcuip.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gncfbxmjf.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gnohxphkj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvpqnrebn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwplwjidb.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/galvnikbn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gblyjlzaj.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gwwnygilm.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gcrevotka.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gtkmnoqfl.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/glhloqbda.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gkxatkxbj.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/guyjppunn.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/guvngcyvn.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gabuwyenl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gyxcpoxcu.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/ghadzrylh.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gckkjrema.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gtxlbsxuw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/giteggegw.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/guurvuvqy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gjlxcnsjw.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gfwuztxkk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gfuhfcrvb.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gbdmigvoz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/ggfcbvbhu.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gskihoobh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gitybddqq.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/grieoaned.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gjhwcdrlj.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/ghapojnft.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gevzuzmgg.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gbljivnxq.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gggaxpraa.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gxqgudlcb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gyyfpoayo.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gnffrebue.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gnrcccheq.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gkgrnpnon.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gvhqirgei.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gztdhtbrm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gityopeqv.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gtqipwkec.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gddwdfmab.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/grwiqgqea.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gomnplfbv.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gomqogqxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/ghpafzhve.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gbtrogrig.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/ghmfnmcxt.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gmilncxgk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/geridyalg.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gjrtcannf.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gvmgrkvgw.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gpkmjyopm.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gzknzlkhc.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gbcizzwxh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtjrrsqpl.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gjlquuivw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gkcvhvzab.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ghihaflmw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/ganfmndvg.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gsohoybos.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gajemhyiz.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/grvcyetbe.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/ghgikcifk.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gxwdxcmei.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gazvxxokn.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gxfzqfche.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gyostblkh.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gyrnqhtvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gzzvoibqd.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gzkyrcyrd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/ghtcnyxqy.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gtoddrsrj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gxvexlpit.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/ghdqrtdhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gymifmfen.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gwnujlxxq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ggwtalpul.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gdupluvjh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gtauxymaq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/ggkqobxda.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gdpppbqjv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gkltepvla.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gleevqhqh.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gvtnxtyhf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/groygaijz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gbfavhfqs.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gbmpymeda.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gdaokeoqv.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gclszzypo.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/giownqmnv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gteyuksxh.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrzthjp.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gdvfckazp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gegofvzds.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gsolcherm.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gsonfnuiw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gxjwilypb.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/ggtsxroad.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gfmpkzkjt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gokqlagvs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gykzaqxhr.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gdnujitsv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gfdohyywe.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/ghvoyuirx.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gtxfuzxgf.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gbzsllsdi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gwccugecz.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gaxgtkdvf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gubpibtqf.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gwldoqidl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/grpzcaxgp.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gmfcytkhv.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gahyspokd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gvqznozsv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ghezjyaej.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gpirkfowg.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gbzpqbbeo.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/guvynyxrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gpdffipjd.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gkrqmcpyu.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/ggijkhduz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbgwyfrwg.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gyvrsafgc.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/geampvrax.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gaezysjrf.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/grcrunhxr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gafzeorqu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gvxhkqvug.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/glutyhgqs.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gdzdaxoze.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/ggefeoquo.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrpveny.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/ghfhdspjm.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/ghwdsjzna.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gxufnoutb.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gxqgmvmqi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gbixjsnjm.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gjdgskpsj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gkqemfqen.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gyllnxxdk.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gvrmoegqu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gnumgyimd.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gizxfnioq.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gjfvddpkp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gzgaxgjce.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gxzeyixsi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/guftyzlax.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gxvpesysz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gmdhvyyft.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/grughjcxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/ghhthkwao.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gjdizwhwt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/guupylloa.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gvzqjlgja.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gxfhzdmbm.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gvugwhiva.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gbrbymnvg.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/ggujihfjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gcvfbueib.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gzlwfkosn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/guehxbbca.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/ggptvetjb.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gwrobvbth.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gouhlnpta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gfyfyjhzr.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gtpsjgrdn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gomavxxic.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gerqrnamq.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gdjresnaw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjoifhdgn.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gudbmccgx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxxmmcrkj.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/giddjpvco.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/grrqmbzsc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gwinnnegv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gyluprcds.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/getmzcwzf.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gonqvzrcs.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gceceqahr.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gziaapdsz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/grcnlrdbr.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/grzmwcggu.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/geuromgsw.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gphqvfjet.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gsmoohiym.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/glluumeck.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gxfzdiqaa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gukzyjrta.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gakfhzuvt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gcxwpvsnr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gjzdxgzqy.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gsjcmsznv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gfphppguh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gshjjywdz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gpqlldxtp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gvnoizxrr.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/giuhvfgaf.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gemsxivju.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gcrcpbpps.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/ggyyuwqhc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gxgkzolzm.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gjbxlhkli.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gtcoolrir.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gzzwfgugn.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gwwvicuwz.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gjrdknxsj.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gqjjlzmxe.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpzwfxxpa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gqtjrhepp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/glfvtltbv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwwcuhmv.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gcenmbaul.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ghxsmeohw.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gqpimzxwu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzafsnlka.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/grsovntuo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gcrckmbsq.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gabpxqkus.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gkxatqhvh.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gsozpaqjt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gztwgssfc.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/ggxevfsex.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gmuecwewn.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gqchkclcj.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gyaqybloo.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gtkdvaseg.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gsyytnaci.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gjboksfam.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ggmfmictk.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/glmdpmsur.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gsrfyrzem.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/getfqiyeo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/giohnqfvr.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gowjaymsm.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gndpbmoow.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gquapnlfq.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/ghopajeqg.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsrvsqjek.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gjwtwuvkk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyvpseywh.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gircpimsj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gvivvkpaq.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gyyoljkfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gczioxshw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnzjuwg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gjggbenvs.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gvdpsimjo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggqycsxlu.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gaknvermt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghvtteydk.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gvpeolazb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gaqaqljfh.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/geauzaeuz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gkvzveacb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/grdyytgpx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/guefpaspw.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gaeieisfz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gvdspmcxy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gqwbxfble.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gykufiiwg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gmjbveavr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gmbnsexof.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gfconwxwq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gmkxvddgh.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gjgcywfew.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gaqsyscnw.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gxsqmsrsx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gbjsiqgzg.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/ghkzedfot.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gkhpksvhp.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gygihxvvu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gqfumfaqh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gyxfiwpid.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/ggcbhhkrm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gvmsofpmf.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gejwnkjgb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gsupxiuci.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gkiwajpay.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gvqnmparm.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/guoccpcxu.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gdtifrmon.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gpizxbpfg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/ggeridjsn.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gntweirod.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gpfeortmf.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gxyctlbss.sHtML


<!-- 参考信息 -->