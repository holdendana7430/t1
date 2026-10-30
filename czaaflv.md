代发 wailian999

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvhnctru.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdbcxhdd.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gwerihyrj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxmlyujs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlydbqot.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxpitoi.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gakwqkacd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gafxubzjt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gbkqlufer.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiuqpxrw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glgxjtguh.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gelyolfpy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkhovaml.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gzwgafvkc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/giaupldjr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrxheuld.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqovyygj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gooxnjqav.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqblwsom.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfjwlree.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gssrmwlik.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkvockde.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjysililh.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gevzuwont.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gzstdizrg.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gomxtlaxe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbncizuuv.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gxljbdkzt.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/guquzlyrm.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gubeoqqct.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsictsplz.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvhndqrua.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqpgfbhs.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkkpmpkkm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaloojxt.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvktihhsq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaxtrotp.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/giqmuhrtq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcdjeujw.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gdhrzprej.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdpsskju.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gxuwvprpo.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gprzqmljz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdphdeup.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvlozpmd.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtwmsdii.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfflhfxgg.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gukjrcfpc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqxpckhg.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrrzvpih.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorndrpwj.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gexxjmynr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwbfygeh.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpogqgrx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbidcnghk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzbcmaza.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyiafkyn.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqwcubkl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdynsbsi.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gyqbdvzqa.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkjkfezm.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gwmarfsnr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxnziwjd.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkjywzsh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjtrgcoly.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxetkqmez.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlvnxahx.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gswqihebx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gorlldiru.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghlenqsex.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ginzxjclu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gznxhoogs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgpzgawq.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrasgaql.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganlvfgbo.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gqddgoeqx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqgudfpm.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gicasyhnb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyijglav.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgirfmji.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiyzjzet.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrusjbwr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlvqpike.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbdbrpobt.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfpcnzfpv.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gezlvjojf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzraudrlc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlzsctdn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gcxyaooqm.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwbzyelf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaoikeaw.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvioundv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqmovzus.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/grpcyvmvq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkrkrlnl.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkavrwwkd.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gccdihqkn.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gvppdfuum.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjmyocqy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpzpcvae.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/guthinntl.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/glhgbtnyy.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdzgiqwz.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gtlxkcpdk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gcfkpviih.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gznpjjgby.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaailjzgf.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzkhqqusv.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwposupj.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxycuone.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gcaxoscgq.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gahcrufep.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/ghjcuqhzr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gldjcjhdi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/giafeljaf.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhwxxtlp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckriuwzg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzodbnidy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvozwdtbl.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqlxqpqu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gexojaaoy.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqsshcadj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtffqawjs.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/glhdzorkg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfcivlvr.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvjozid.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdsbkax.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gajojbqob.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gnyhmwfdt.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpaweltj.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkqokwop.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gpesylrxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/glljafjyl.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkjpagjv.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ggntmottb.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gninwquxi.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfsamgah.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvbfqypke.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gdzlfsvic.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gonsinwjw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gawqvqzgc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxuizboh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gymwglscm.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggynasqyv.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gwujvirsv.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnqjxemls.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gjphpybmk.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdcdizxo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzkxwrbb.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbvprojka.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatddzroz.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gyswlgnfo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gbfyjynmo.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwvyqzocz.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gnxaxtjve.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfebliudi.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbndsgbnw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gquaxmkpp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpfmdjjp.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjfktvki.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gjojcoyqt.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/glomglung.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzujakkz.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbslutjs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrsjeyyy.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gqcntsqye.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngbgaxqq.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfdiudth.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyisokywp.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/glfgjwhqy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grgcctepk.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grrrfxbzq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejtpscau.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjteetqo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgamlmvg.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gslrqlluz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxecbeov.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/guysffynj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmvcetgjs.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gflirtecd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjupyupze.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gcpfaxaae.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvplshfxa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goisslnqb.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gfkroqhps.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggfalmzvj.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoccbvfr.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzyfnhfk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhiotaus.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwijkdkbb.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gckzsadxn.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawmaskus.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gdnqnwifj.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbgvowyc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/ghmeeillx.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gitatyona.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gebnnyouc.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtiqnlzfm.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/glhfrpuhl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkpfgqyd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gjxeuafyk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gtizfqxwj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gqeevuorx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gimvoubzl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/glmwloshg.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gcoealltz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxskgfces.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcehdlleo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqltkakf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxjawnyl.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqujblke.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqppxejl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyhkhtqu.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gbgujonqe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gugtzilbo.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmawuirt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gcswhafnq.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtspberrt.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggkvkizhi.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gumltpjga.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpefgsmfg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggxnhhxtd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzofhlzwt.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gogetgqui.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulczefws.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkkgflomt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbrxtpuyl.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrqujlob.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gcxwzfoqn.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeltygjh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxschcwfo.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gyieztbrv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gfhulwobg.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ggcwvzyce.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/grksfhycz.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhrggcku.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gargfhkay.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyjrokls.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclyhxhjw.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyoiuysj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpynnkkbu.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gpwrutevr.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gijntquwi.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxkhngrfe.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsriifbh.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswvoebny.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytjchhzk.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjqwcfgo.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/geztdtkwx.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gyomrfjok.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjsciuh.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gaxstksdf.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gazyxsyqy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajrtzcpr.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glcihighe.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjmvxulv.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gbtbcpgzv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqvqscoq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjumrspsr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftllwqjh.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gaepispnm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtboshvyz.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/glrqzsclf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkckngly.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gbivltpny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnqguhtk.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/genuxhbwh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gthlgzqml.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpezbpjfe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gzpyvgbjw.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gyaauleaq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/guzfqojhb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqydpgtoj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggixxixgu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggthiesoe.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhtgfbjz.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gtppanrzy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gjzrusesg.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwqobeov.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpskbrupk.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytqgofsg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmkrqlbkp.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbzfgoscd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/giqaxpged.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gmweyyjbo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guintmgiv.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkqsobjyk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gnlttydgz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxfhzourw.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyqqcmfp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlwhqoqr.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpulfhdn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gphrqazxr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkitxfjl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gishmsuok.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gsamtcjhf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvgybjmt.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gopoeftci.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgevyvjb.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbuwovuu.sHtML


<!-- 参考信息 -->