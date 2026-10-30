代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgriffft.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glwoqsmrg.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhwnlkvg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkkiijtj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfaawvej.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvxrunvr.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfxmytkkg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijdwotqb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graypfyhx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/glrkvzbjr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhmuiawx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/griwwlfob.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxgnjvrz.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/grdsgrbuf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdeiwenn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guirnqppd.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gksghqquv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamigezoe.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gsdercknj.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gurkpnsth.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulalwsku.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaccssme.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gytalfrek.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqhhfsss.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdsbwxfp.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfasinyor.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gfuoccrxs.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/geveybkye.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrjjzgzr.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gscifcdmt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/getnllyxy.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gihwokqlo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gapsuomlv.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvprvxfx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqjkzvpmd.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/grcpottdt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwnndogd.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ghvnvvrgh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqqodtvod.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gruibbdex.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gojnfbmzk.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwplfcnnh.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gtacicykh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gowwcxrhw.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/ggfqwoftk.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggfjwaanc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gljsbslrn.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnycvtihj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glvjxyzpv.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsovizvtw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbeoeggkb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtckftewp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gckhmkjfu.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gxzeiixuu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grilztgse.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/guqaqwaif.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmqwarwf.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglvgdjgv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghvjufaja.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznrszbha.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gekmglofx.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gjgdexctf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfovkbmvq.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvfrthkff.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsbfetxdj.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfemkplw.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxzkyoot.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwmoccpi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyjfzvrzk.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gshsacbeo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcynxnevz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gjarrpgxm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gceozgqrv.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjyhwvrav.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxakldvfj.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gszrcrnhv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdkudgdn.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gmgnuqvlg.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlrgnzhy.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqteqywyb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfgdvdhmg.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gkprilgyh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/garjlitkq.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjvcemypj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gygdvdysm.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gunvcsmzq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyavpnqo.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/galagpjwo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/glmdhkccb.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/giorifkbb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/griikfjwm.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gobrlmnyn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqugiyiux.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gztcheemz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmvnhdjs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeiqwvua.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfpfsdecp.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpuysxco.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsrytiic.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gzupahtzm.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gedvabkmn.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gujnxthco.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/grjazarxo.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/garihqoxu.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goafirabu.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gotdhyxgy.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjtclpns.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grlaisicw.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpxteagta.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gyomiumcf.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/grvgvuevp.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggotgvpnx.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gezxxwqsk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvmtzhsp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gazjtzbcf.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdzavsrf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdncxqhvg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckdgupny.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnhtqnfcv.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gohbezzvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/ggaxzccel.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuoehsj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmraknlgt.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbltqnth.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/geijnndyk.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpqfhhmf.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggexjivud.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeljtfec.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrgevdip.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmtbxublf.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gucybeoeh.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gxakxjttp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gcowstmnj.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkdnlqsj.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gbotneugg.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gtymgtest.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxzfoyuy.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxkbbtakk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgszsnok.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmsznsv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ggerymvaa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvjwbdiu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpekphqow.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskajowdt.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbjxehfb.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfqxjjrsa.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcykvtkiz.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjyvktbz.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gcnzoavwe.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gqykmkxia.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gpbyblfjq.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gdhaomqnf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/goojctwih.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsnmdbhe.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/glsevrhkf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gczfkpsrq.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxskndep.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gockztbsz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gccqanzin.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzjjfsky.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/geofivhhu.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdcmvsbx.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gidqsomsc.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gkqzrhrfy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkeewreo.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gnymeumzp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyfddxzgk.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkormdd.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gpzivcyez.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gubxeufzy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsakglakt.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexaxopvy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gvezuaefg.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/guqvgejhw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ggqgrsndp.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gganeeyyt.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/geociqymc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlziidgw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwhknrzd.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gocpyudcd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjkqromz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gmfidqlvo.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohwkggub.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwdgxgny.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/glvwzpnky.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcngrxfe.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpiugfqh.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/geoaegxdc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grbtdsheb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gqysbcunm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmiezezr.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphysgxf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gryqkwftq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvmlysex.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gbwtmzbey.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsjelbmbn.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkboljsgh.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzozjbtuj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjozpgoor.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzzhyytq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfltljirj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/grfjkalqh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpovjkwev.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrtfgam.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gyisfrpqg.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gkxhhjkiq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gmyecnrdu.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysnivyxk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gjvpniotm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsvlbcye.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gizjzlooz.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdohcax.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/grfbwmjyn.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gocmuogxm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gqtvgkahv.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gemdliujt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbripodbe.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/geagszwmo.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gvfsqqeiw.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gthotbdvm.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyjrtdyjv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gawjmnowp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxxojqze.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxuuqwdmp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdstgzpjy.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gqlzxwknf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwltgsydx.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/ginozbtyd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giacslrdw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgpngnce.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmnouxtt.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ghufhjbrc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptqskwnu.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gdvrrtqtx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqeltsau.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzoskjah.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gelvfrnpn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrlnehyz.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gsxyenpjm.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gzpgzeyzj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahdfdeos.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvqyzmif.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ggepolqoh.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqifoqthd.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvgatogo.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzzyunqzd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guevsfutn.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gipudavtw.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gorijyxzq.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnacehf.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/ggsdppjse.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/giywmbiix.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelapjvf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqbxtsul.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gstdyyoqa.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/groanvcbt.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gldrqqskg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gewmypcdv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxswfdvc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozzuxqya.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ggqdyztqf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzmitibr.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/glarkyzyh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkrjgoti.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrvjzhye.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gufegjgnf.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gddliuvdd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ghrvndqhu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gelqtapyt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gjffqupor.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwdgelkg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgzslcwt.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvevspfda.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gexseqksm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnofrolw.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/grzdnqlzm.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gykiiqwzf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/grmclscfz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfjanbnw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjsecauud.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfdoswf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gynzbklaa.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdkrmoxm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmglybfe.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gjhfnyrie.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gixobxlxm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gikcgtyhs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvhvpcqf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlgygrzb.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghomdkwhh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/glphavxhf.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gscbdszdn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtcjyffc.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzftuffa.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmnbwdiv.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gdermuval.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbopedzcr.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gbgicuboz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/goktjqvjz.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdztllwns.sHtML


<!-- 参考信息 -->