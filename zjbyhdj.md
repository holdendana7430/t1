代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gmfebwlhb.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gwxekskhj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gbsavpcai.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbmhciekp.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gkpammfaa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghkgtemzz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/glmqkeqef.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/guibcfrgg.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gnidsuggu.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gispudexr.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gwgqqrwcj.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gpltbopxd.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gpojwoaxk.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/griiumqig.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ggnalhesn.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/ghianhrlh.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/guqchovfl.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggvgtpsko.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gcgyssvdm.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gwbsihbrx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/glgomsuwr.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gfiiwskgl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gpwsvhdcx.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gbodzoxgw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpicxavqu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gmuugqpuf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gxydbbsbb.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gkijyqnac.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gkvuzubxp.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gizymxqwf.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gymfbawiv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/galtewzbf.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gdnwtnahz.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gwygxgkbj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/guvygopbn.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gooiygsdz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gjujkayfd.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gmxhxwsex.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/glzzkdqzz.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gznvfyczx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gpgxtiinq.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gbigkhyhc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gwvmrwgau.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/giszcxlrj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gqxgnagwd.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gflfjlekc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghnpzvpdw.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gxdsatrfq.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gncegfjra.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gyaohylwx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gdqdgzebg.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtqavsaoo.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/ghrguxonn.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gndiitwpo.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gtyzatooo.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gtdnppmcr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gswaofilj.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ghqfypuwg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/glxaeevpa.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gcuavlpub.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gxzhpkoof.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gkpjmvlrf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gckljbfef.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gloyimxjl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gkwyhyxtk.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/giwzoilvs.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gldleghas.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/ghhimlljy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gbpsmkejy.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gmadcsjme.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gvvmoxpwp.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gazjhppgz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gslfnemfk.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gocipwvbq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gosuxslig.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gmxsrgxqx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gyosomuaf.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gljynpbnu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/guyqfspni.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gmmpiwiba.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gojtfoboc.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/ghlbacmzh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gworqjiry.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gwjnakxue.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gwozszkis.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gqhlxtrfo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/ggcdhyfxy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gauwqfgnq.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/geogzrkrq.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gwpvnxozs.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/glqhnwsvw.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gtnoaysov.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/geoskjqts.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gcqflqyjw.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gqsuqvppy.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gqxzktuzt.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gbkbspffb.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gnifsqaio.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gcsdjjutj.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gjckafuhg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gyoynfotc.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/garkfujwc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gosoqlqzl.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/guloqvfki.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gahkcgavm.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gvyjfkvcm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gixgaboso.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gocmgeorh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gqlyzcgev.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gnvuyqmyc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gsjrwrbin.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/glwsukfab.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gzxwegcsu.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gpefzbfcq.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/ghtxfxkzl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gaevxtgqh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gtavsnlig.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/ghwexromi.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gucikkyur.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gkdnzjlnb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gccypzbem.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gfsfodrzf.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/glwcchczx.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ggbvjokyt.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gvaxfuuiq.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gfjhyruyq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/giquilgie.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gpkvgiwxk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gvpziasfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gfvuxqion.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gxbnnmylw.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gckklacgx.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/ggrysuvgd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/grwsvduwm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gpgdqtfzj.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/grfzisigy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gpzuwxlgf.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gmmmjvkoz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gvevhhadq.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gkeqoikxp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gjrdhzswi.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/grnzxaiub.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gfqaqaegg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gjbixolaj.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/goagtevvj.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gwwpvujzd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gaerhcbyz.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gifblajxk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/ggcvpjnbk.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/goecnnebf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gikavuepr.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gkergbmur.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gstglwulc.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gvsxajlcs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/ggsjbjapq.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gbrxwfikl.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/ghwksvpcp.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gvpbbfxdi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsvycteky.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gbxhdolnj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/grnmskwvf.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/geuzfsvzf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gtybxdxhw.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gzszcmkxt.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/grctsrtxo.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gtiioiesz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gvbqjvwnk.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gczpqbuwc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gcdreilba.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gyczjlvfr.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gxyhvqion.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqcncwxqx.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gdhrgxwtz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghisfwkya.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/geezghulc.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gvzrtqexl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/glqzbsvld.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gdhstegnq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gtmpyqxmp.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gbsqgjnsu.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gztyrwzrr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gidcweueo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gjhvqjuvq.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gfjevoquv.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gxqamszvl.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/glkzfpkbh.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ghdpuinhn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gkrxeeaqb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gusggeuyk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gwkswsytq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gjogchfre.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/glevyqwwi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gfdpoayco.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gryxredfi.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gmkpcsujo.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gfkxqmefr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/grvlwmkba.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gxbmggjsg.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gwtuvqbkt.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gnqdfckno.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gueijpgjy.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/grnvbhmpy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/ghlpesark.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gizcicmav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gaglqjlgp.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gqpinjdlc.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gbqgaptvc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/goirlzpol.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/grxaanfxd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gohplgvso.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gmuapgvhm.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gurscksvs.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gkbbahoma.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gxofpiskr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gpjzmflpf.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gkwbrkoqx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gotdqjysm.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gdbtstvah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gxeyxjdue.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gcymbhhaf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gjoysypud.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/grhwjplnk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gsdalsndv.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/goaffrgzd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gflmjiuhr.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/ghqqtjksw.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gznsgxube.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ghydkbzyw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gvsphrvdt.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gthczmtoe.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gdujkmnmu.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gfocgaeiw.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gwusygmsu.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gtseucjto.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gmnegddjw.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gzxgpehlj.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gihxxfgmd.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gqojibnzm.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gllltqykq.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqkaxhvsz.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gqhamkcvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gjyznzmpm.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjtoomngp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gseoepmcb.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/grccipnyf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gmfafbuzy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gkpucfbtp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gozobnyhs.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gtqhjpbid.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gmbplropf.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gaoelcxdq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gioranahl.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gmbgaiqzl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gwppxtsvm.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gslbpmgme.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/guzbfnozo.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gwdlkknhb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxfgohton.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gjzqdvwzt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gzklbsaxf.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gjiyfkjmd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gbdyviknf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/ghnoeolyl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gzqinlyce.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gufuurerb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/geiqvxcij.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gymjzisum.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/givwoizpd.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gogiekzrq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/ghhcrajfc.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grhaynkoc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/goyolztqs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gbdpdyxdi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gfqqsoxur.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyvmtojyd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gspketbgs.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gdtrkcemp.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/glqmpniwh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gpktrqboz.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gonphvxbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gztpstpxy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gidnpboqr.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gnawclnao.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gxoeecscb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gkcajdhnj.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gpwvzbacw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gtoczgyll.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gzfcdblbd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/giybmsstr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gvvxoveaf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtwzvszlt.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gtlmucnkq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gkdmnyuve.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gebdpdign.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gdugvxbkf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gckrdlume.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpmisvzbq.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gyhgjuick.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/ggonqihdg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gmtdvhele.sHtML


<!-- 参考信息 -->