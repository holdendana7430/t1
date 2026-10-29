代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gzwwpevoz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkgyihxkg.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqakalbor.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gusrydkkm.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gvjzwsxxm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyczohqqb.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gcbmrymdy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/grjggzdiw.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gfohmwras.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gqhlbhwud.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gtvvxglur.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gtaxwryxa.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gcafwumea.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gtasvakhk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcmxcdric.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gcybsgwcq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gvuaewsii.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/ggajoeleo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gsuqcrsfx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giiqxfvjb.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gijgamsxt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdtdkjjda.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gtpgmkohz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gbckrrghj.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gknqnxrst.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gbmmabycu.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gsniwwjwn.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gnprzjznk.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gdjvzerlz.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gxtojfwnl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gaywwetnc.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gfujkmqgp.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gokjxnibi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gsuowajrw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/glguimnsr.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdtegsxvw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/goskstrdi.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gnwntdlaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gmadtfutq.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ghteipqta.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gnykvxdlh.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/geqymhkvk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gaxufqgdi.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gdekyhorq.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gptcxbyit.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gofzgnbum.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gxdyahnef.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gppcgjmew.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gkxwitoku.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gxymsfdpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gdmtcxlcr.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gjzjhfnvt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gzxautneq.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gqxkupudx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gdfvwkcuw.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gggrzxojg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gpemsfrcn.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gckyrrqvq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/guczdpktf.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gdjvsrovw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gwjiyrsfc.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gqqfsfsgk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcavhgxcs.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gerjzyimx.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gcmvcyydm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gcablugzk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gxozamvsv.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gizkdmmms.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/ggpnwypnf.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gvhzrmxwd.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gdfdctdxv.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gcdnozxlv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/ghjrcetcr.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gkzptztmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/geoivnueh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gndbqptdn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gcdgwucpc.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gfzkervvq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gmhsnolld.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/ggmstgpnc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gwifcaihk.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/glotwqxro.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/ghklggntc.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gebyhjeow.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gymigpfts.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/glzhzfbxn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/geqzugxea.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gegjvuvct.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/glxgzbxps.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/geomvdcmn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gyildxfdq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gslyvzech.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/guxgpsviz.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gsaxkzjit.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gamoglyom.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gwelrcfgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gpknmjvhw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gbiuznums.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gujcuzkty.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gvzqyfpew.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gidxkstdt.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gufmeqhrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gbsqnkizu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gboonckeq.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gslktyeov.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gpwztowks.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/glzkmgigk.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gwjbgfspe.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/goaxjjqed.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gwlrvkwqj.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfxtbcjtn.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gfvadspav.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gowsdopzf.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gbyytmsoz.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gmykwhwfl.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gybgplinl.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gdxgrcgdc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gexusgsqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/glngpikdr.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gobysvgna.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzrdebemt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gtlxsfets.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/glzgyigcn.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gkydvbitb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/grbwotrnh.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/goatcphtn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gemkljojv.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gsdmpidme.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gdbwqehcf.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gjzguwjbj.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/ghewvuavu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gachpxsfx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/galwcxklx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/glhtaqlvk.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gqosnzzeh.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gncwrwgsw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gmezbjurh.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gpipnsddu.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gdkxzqtkw.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gicsuzdud.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gojgqvvox.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gqmuokepg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gfpqbucgo.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gssemnzic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gimubtluy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/glymrspgl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gdruwulkm.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gbxlrrxzq.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/guevjoyqr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/guyjmorsv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gwqmuyswx.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/glcvzvyks.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gcihpgfbi.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/ghijjhxwu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/glwrqhhul.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/ggiqfoozp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/getwwbbye.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gqxlznezd.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gzdyikspl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gxexbcpuv.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gulecrmvc.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/glicgfvpn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grnhffrtq.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gbfiknerx.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gyhcqalco.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gdvlzlxno.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gyflewznq.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmcgskwta.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/ggsusxhwn.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gcfvymwtt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggpdolhnu.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gokrpsbtr.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gluinnich.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzeoaefdv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gamcngbqx.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/ghadmwwlx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gsaymxnje.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gcpfzzrre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gjslpzupf.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/grcgdaivh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/glkubxcpl.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gmfkqwiej.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/ggbbdqtah.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gygbmghuz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gmmbddxyo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/glvzqchpv.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gsxwpqmhp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpllwtxbd.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gcchjcykw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glelljswp.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtllcenfd.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gpxqnafhk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/guqhcgixv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gtiubhxhf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/girqzhddh.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/grnxgewus.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gpcnbodsf.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gjwkhxkbo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzdpafcxo.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gxdommtdp.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/ghpsgsbkk.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gjmvrcvpb.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/ggvditzyi.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gsviukrps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gftcxivjg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gipmynqjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gpeppwtii.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/ghvywvfpo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gaargyisn.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gggekfvcu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gcmmsfxmq.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ggwtmudvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/galwenbrm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gvlltstsc.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gutwiopdx.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gdwuuqgik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gvacmsxzz.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/ggjroosae.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/grwptcylo.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gllwtrjdn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gtcegwhsb.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gsgxoitvm.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gqxjvpxul.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gkzmumobd.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gupbflurn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/ghcqupipe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/ganfkpazp.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gawjyuesh.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gsaikunzg.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gxdkofpcp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gnqjznrvl.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gzfchinyg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/ggfpakyoj.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gqouzguch.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/glstruyqp.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gemwyncio.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gxqgvzgzz.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gkugmmsah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gatvvqkmo.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gihmfkhnk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gzknpkvpz.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gonnrkcgk.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/geduolmkn.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/grietjtpu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gapwsypsw.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gpkjculoy.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjihyqzwo.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gteiahpjn.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/genrbxkdg.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gkgbzylzh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gnhdxfynn.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gbadkhibt.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gncetvjlu.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gsfokyvzg.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gwvmevawi.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbhzupqhu.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gbxquioij.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gbmsrdfxg.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gmjsoaljv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/glvrtcpyb.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gfmmkeztl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gonoajwlq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/ghshxyzxp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gnoitkutb.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gsygqtlwl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwjmlgtxb.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gdsabwzdd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjmmxxwre.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/grdowzrmr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gpwlredgf.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/guwdysvln.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjhersuxc.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gelyezolf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gsrczoifu.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gixzoqvly.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gybzqnmsv.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gfysbqgbn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gflozomus.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gwcilkvru.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gnmiprhhp.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gsuxgbmxh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gvplhuqyx.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gwcjuuqid.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gqvlkzmsz.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gwlzjxzsg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gmgebfzmv.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gwieimqiw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxquugfsy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvpukrmrb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gvpxqmxrm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gjyshwlfu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gfbvfvgsz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gymqsbuzc.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gdtaahnqp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gensjmukq.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gzovbvamt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcxtgnzrk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gtkwvkqgr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gztocgnzk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/glfukfype.sHtML


<!-- 参考信息 -->