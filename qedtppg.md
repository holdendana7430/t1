代发 wailian999

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gwjpavway.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gaseyekzs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/geztvwmrm.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gqfxrcaqo.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gpjqsvxix.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gmzotmgeg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gbbabqpfs.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gzwvpgraq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gonwxqjca.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gsgiverma.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gptmerply.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gmedlkiwz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gbnwnwffy.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gpfqucfch.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gtauwowfk.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gfnnklywr.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gjzlxfqqv.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gpnyzsfzj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/geckqhauu.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gvxlnwkjn.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gknjcxipe.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gsfhuvxhv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gpvnufikc.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gbfilqrza.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gddscxhtv.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gqtsgeivc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gwmogedye.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gxayqnfuo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gwgaaslol.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gedgxxqqo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gbhrbfkes.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gdjkfxuex.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gvquyglhs.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gbrwvonzo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gpvlshpsp.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gaewmjrai.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gmxygorsb.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gkwsjnbys.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gpomcjaji.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gjrhdfgph.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gguzfunlw.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gnawehrqc.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gtrxugaas.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gxligkvmx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gzadkgcrr.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/giknhruwf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/ghjblealk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/germltzdc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gccoceggq.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/ghbfwoccp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gvqcuyyau.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gdrhoogvd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gakyivjty.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/ggnjjpevm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gmreqkozk.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gpdextrza.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gmyxurwmg.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gkzozffmi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gmnxovxax.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gocprzbww.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gkrroacuw.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gahrycuzl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gssempefb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gwdguoizz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gqpeusikz.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gxaxnfjtx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gtthtduvk.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gmjwsgvsh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/giwcvituf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/ghczemabu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gyasfmbud.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gueimmqoe.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/glrdkkafb.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gmpbqiyrb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gzyheclmo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/glnzcjiut.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gnnernhcs.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/givytodbh.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gnkpvsjqf.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/ggdryhpwl.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gnfbgsfxi.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gctiijkbd.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gxejydcuk.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gaumdiqqd.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/grcvxvyzq.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gpynzbnqy.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gxltuoinq.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gheserogc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gyzrfsykv.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gqgfjrbcl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwzugroan.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmssxky.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gxcfnfkik.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gkwdyikqg.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/grzrtpsdr.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gwppmwycm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gbupljnmb.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gvgeiseit.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gfxujexog.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/glnxouolz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/galolfgus.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gyigylxfa.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfvtkjrsq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gsdwapyzc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gfsfydbir.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gijdtfidn.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/giuwxmcid.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gladvwcsu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gdaiutoyd.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gfibahbvy.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gngzarkog.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/glidbtvzt.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gntopwshb.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/glqahqlxr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gtxmjtujs.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/ggfkzhret.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gpkjkcwky.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnqnhiijd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gxgfdpyqd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gbtyaksno.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gdafggsov.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gtrpazzyb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gobvgvzus.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/grqcimzct.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gurhmdsod.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gvyxfgzxo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gqxhaibpo.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gdcgniwws.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gagsmhrbp.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gfabxuaxd.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gnoklglll.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gwqklkzpg.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gbuhjiimo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gcpizacnt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gescujqdg.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gmmwcckvy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gaprzsvhp.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/ggwvrwirq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gjgkaxncn.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gxwbngzih.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gavjbwike.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/geuqdkghg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gfussyddc.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gocnxbvgj.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gripuckge.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gtlnjeoml.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/ggzvdvyiv.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gniziojfe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gubukqfbf.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gwcneehff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gtotvxjoo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gxfqxfbrs.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gtuqvnpzz.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/ghsikluxr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gvwcgqnqt.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/goczshsld.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gdqnxpuhk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gftbagfdm.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gfxgfelph.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdkwpoojb.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/ginsmnevy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdasxwban.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggikkafcn.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/goynztniv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gluprxtjo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gflgdrgsf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/glifxkejw.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gwhrlnzbh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gqexxgtpq.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gyxmkhtfi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gqdxdmxdn.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gzprsdckx.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gtbfsdfsm.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gywanfmgi.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gorivezcm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gxtalnomx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gnfztqkwi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gqkhrxaop.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gamudjmry.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gxnxaqntx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/grndmicii.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/glvmywtzb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gyfbynjen.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gdnijbnyi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gtjqkgcly.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gpxbtrmvk.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gyvpkpusw.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gnxdiorns.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gzeirkxnp.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gxjhhvvtv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gosyxdsff.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gomcucabt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gooepdhby.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gkzrqznmz.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gadhfyeer.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gpdxflgcv.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gecnrthbn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gkpzmzfde.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gweybfdge.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gpxiwvezf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gnagzqnzd.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnhhmnzvj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gxoaxyhfv.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gbmhjbggx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtqahapnx.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gutdekiha.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsjbfaem.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gdusrftyt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gjqfvpdnq.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gyhuciyiv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/grqsvmkza.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/ggpzhiida.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gtoqvxspq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqmyxjaii.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gxgspsdoc.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gzlbtoiqq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gqenmgvbp.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gvihlketq.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gexriorck.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gizyephuk.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gjdqpyjjc.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/ghyitvzea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gekdfekck.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gfuuqggms.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gfjklrmtt.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gjuawkzpl.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gvnrhttzp.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gaitttjnp.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gnhudryqt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gqobxuwbn.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gohzegpag.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gefguvpog.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/ggbltgaeh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghutbhcep.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gxshcaowy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gqgjgwder.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gpihdnoji.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gcgfvoxmq.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gktugwhaj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gigtnugjh.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gulwnwwri.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmzbudvfi.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gnksyipiw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gqfxrcplm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gvxggohzj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gjfrvuagu.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gaibnsdwd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gammuxwdv.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gerozpizs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gtlmgraxr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gxzslfynp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gvgxpavyv.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/grvfqnqsa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gafdkgort.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gctobnhfp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gjwdahlpg.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gherneahk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gdimpwyuf.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gpcleheex.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ggetfkgxx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gqfpucpug.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gjfbdmtqx.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gglprlokf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gdgfgxsbp.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gldxlopls.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/grnqdomzb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gfemvzflz.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gdzosndkp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gdqiirqhb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gbhialfxy.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/giyuudaxh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gdruruviv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/ggjgbmafl.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/giixvqezn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gqaznwktt.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gmvvkikio.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gobwhfqfs.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ggqcaoihc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gicucylom.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/grfgkfggb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gkdmsvudf.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gqmgvhwxa.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gaebjtnof.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/ghnnjtqoo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gpanoynjo.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/ggqgiutba.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gpcsnruku.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/grletcqot.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gpklnzgop.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guzskptzp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gqcxrypjf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdcpyapn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcwvflaqd.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gzffylewo.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/grlsmyqmt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/ghjklxpil.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gfiiwwdvy.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gvvmmcuxj.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gyuqhtpmr.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gzlpeiawn.sHtML


<!-- 参考信息 -->