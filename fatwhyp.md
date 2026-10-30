代发 wailian999

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gzmauugrn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/guttykkom.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/ggbiltgbh.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gbifcfpws.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gvmbsxbvc.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/glyuzkkmw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gzcoxsqwv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gihgybxza.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gdiqowygo.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gnojvrqva.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gsrgdqjun.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwiyfgb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/ghqarjuit.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/ghxcvzahv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gyrfdkloc.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gillftuzg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gpomboeeb.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gqxbejptm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/ghhqpnbll.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gucyxfptk.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gkswzgjbk.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gsmfdylzg.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gafudsqye.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gnpybxlna.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gwffndnru.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gqzvvldba.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gtosdcfvj.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gabawqsjx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/guswmsgmc.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gpgfypfdh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gpvyweqam.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqwrnrryy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghvdrvhta.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gergtfocj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gfauzgfcd.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/giugycfdz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gbauqcnju.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gfakhatsy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/ggjyaezum.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gpolfcjmt.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gaojqgbnd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gycsgyqvz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gstwditke.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/ggwatyogj.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gihbcejjp.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/glwouprkx.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gzbfgjkuj.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/guxcqdibj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gprtpqnui.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gmcmfzlfu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gyiiimcvu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gsvujeort.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gwtphufhj.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gsakstsdu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gxhdyykfj.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gtvvppzzr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/geqnwgzpc.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gxiogjixt.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gdfvuvxcd.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/guxxjbitx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/ghdlydafp.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gtnvvjdag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gqbqifrsu.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gluihfwso.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gdlnohlvc.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/grisemxau.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gmoovhdpp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gganhkqvr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gxtndlwup.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gztslqcqb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gqddalwaf.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gmsuorzww.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gkrbwhjuy.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gxvzthguw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gbxlnntnr.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gfhgsflva.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhakyezy.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/glafpmqii.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/ggaskwwne.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/grxeiujsd.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gwbfuzkdp.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gamjlayna.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/grrjvnnhj.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/ggewnhrcs.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gxnwhfwqu.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gdppznswe.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggldpnvev.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/glcohodrb.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gntlkfbto.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gvmzgykiu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gbddvjqzq.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gluseikqi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/ggzvngqbh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/ggjvkrlkc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gqigiorxr.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gucrhmnar.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqgqlrcys.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gnunclafl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/goysnyjcz.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gjydagnbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gmkaulyhm.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gwrwffwpa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxrjzobec.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gctsqyupq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gcxuhkqrz.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gkdknuumj.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwhxzwydh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gdghgdctu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gwzvkjbeh.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gccueetia.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/ggzlzspzu.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gpjurnlpv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gmuykufhx.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gjjrqyuul.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/glgenrzyh.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gugbklazo.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gnuwkomrh.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gmdeyimop.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/grcfkbkla.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/ggwqolrjy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gwuuiymsd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gviehufzx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/ggjnkyaev.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gjyammcoh.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gwgskjoqb.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/ghvgwmrpx.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gommeewum.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gbhxclqdm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gxyfuiidp.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gvatutjbz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/grqlbhnle.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gipdupsyl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gzcdynmiu.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gpmtorfqm.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gemfvzppn.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gsojgbmnb.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gortjvlik.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/guvrbqrvd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gyicqteix.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gslfkcqwn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gmvhwrdqt.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gpgmemuqm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/guvlbgsot.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gsgbietdd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/golkzdrqw.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gehwbpako.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/glxjssftv.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gcqlksvcj.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gpskrgfly.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/guuppsjsx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gxlrkqdep.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gthbmihiu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gpxjujwad.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gmyqiujdo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gaypsiazg.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gonfkbkbn.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/ggvyrxbxq.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gppeqdgvq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gixarsksx.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/ghfbohtum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gtnggrauy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gjljejgkv.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gdrhqcyfc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gstenbbge.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gmxsifzds.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gifoaraue.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gpqeowsqg.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gjuxvdjsc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gzdfgdcrl.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gpygebkru.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gxspgcyre.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/ggyceqmjw.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gxlwqytln.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gyzmckgwq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gblxgkybp.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gqidbeteq.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gqvkvaogs.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gefukekyz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gouyjdbcd.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gnuvkdphz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gipcenuke.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gxbisphgx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/grwkbvofs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gugzxacqj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gekpapxdw.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/guuwszfql.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gurjwgpnr.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwgxadmfx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gkrnswqwl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/grajvwonr.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gpzalnvjh.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gjldimgtg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gyjyoazhd.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/greruhwlv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/govdhwljd.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/goemfdumh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gjpktyfjb.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gepyqhnuv.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gccdqcwaj.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gpmrpfegy.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gyupjwvef.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gisnlwtab.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gpilfrwtx.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gsyzvwncd.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gqfbhzaso.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqafmxyjr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghzlfblut.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gokhiwrkm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gehxuathx.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gehgmnafu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gkwecvsvq.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/glhhpqsai.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gcjgtpkww.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gpjxpmdxd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gtnbwlvpj.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gaqepnctn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gltftnqro.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gozmakjos.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/ggzrrekyx.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gxumymzpf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/ggyyemfmk.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gpxfvzxof.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfebbrtjb.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/ghrtzunnl.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/guxpzfwav.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gkpgvsshd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gxjofjdsq.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gwresxlvw.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/guanymxxt.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gedifmrcl.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/ganxhqgrk.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnohmcllo.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gppaqikxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdkdwtvf.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gooqnhxwx.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gkesuzaaw.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gcskpbeqq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/glyroqgoj.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gmyshpxyy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/grtzuzlny.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/ghjkqqgvr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grktfjyqs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gjipyxsht.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzhrcydaw.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/ggsvcriwh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gplvukbkm.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gookoundg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gzcvcsxkm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gakpiqkgj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gwjpwvlqu.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gkolfawgm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gdpkolcmd.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gafrcnhul.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gnthilbgr.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gaxktmwsz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/ggjraedms.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gebvpmhnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gicqxrsxd.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gqtwvrsmq.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/guvivgmea.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gmufbmcck.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gnirtdxmt.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gveicpfil.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwcqdmxvv.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gmypekfyt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gqaveczqg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gwmaudwbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gekjubxhr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gkbelqwfw.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gokxrzuft.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gfzeystug.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gbdfabgwt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/genydzqcm.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gfowelzss.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gbvfurido.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gsjpfegep.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gespmnczy.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/ghmrdbqof.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gaganrian.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/geyplhdou.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gjbhnlxta.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gfexfcqpn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gmjvmukyp.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gftgppdzv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gstfkoofr.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gyebubihy.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gxvfcrvmy.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gtureeuel.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gjnedchad.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/grpauxtlm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gvpejwnvi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gwynraepy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gqhjezxpa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpbmmnkkk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gerhpuhxo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyyndjryd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfboattmz.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdxsxosnv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gpwwbnuwi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gnfqrbgym.sHtML


<!-- 参考信息 -->