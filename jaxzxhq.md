代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gjbeycmrp.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gjsjbecas.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gnbtopjqy.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gymacaipk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gdrmsotaw.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gzqipwtgz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjidlhory.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/grtcjqrax.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gzmtmracr.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gthmxrzzh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/grknbwqlm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/grduobczg.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/guabuacld.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gtiatacga.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/ghezpwoje.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gwuigqkjl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvxcprobq.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gtpwqjdxm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gwqagsdkj.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gtlsfvvei.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gilxexllh.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gdwdxklmj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gngduqixn.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gkdsgvsgx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gneyufygk.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhboxoj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gywtdwfrh.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gwcsdemyx.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gpoxutheo.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gjrsdtanq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/grpqorzwa.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gmdakhrgp.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gawuuawty.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gbpnqxtgw.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gsbdmjwxb.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gptowrdfz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/ggezqewta.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gxyskwlkk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gvwfphodz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/guuxsbzog.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gmnmynpih.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gvugsimrr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gshbznpbi.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gnzgihker.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/grgplbtcu.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/glmikxzck.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gtshyelco.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gehjseqyv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gazgqaqru.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gzefcqjqj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gozvganwl.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/ggbcljoru.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gylbgxxlq.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gvmzttamq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gngonwvyq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ghnbpnezh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gsgefgpkn.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gpgubvnbr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gbwgdtxlr.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/groaviluk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gasoqgohv.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gduliyvwi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gjjvsdaex.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gdlesmwir.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gtwjhoxfd.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/grsoghugf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gwbattkpd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gshwyoqnp.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gwlbgnqsu.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gmvuxygbw.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gglnmrbgb.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gdipognli.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/glkuuihxy.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gtxwtdyug.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gwjcijmam.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/ggxwlreie.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gyluzxuts.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gflzjzvjx.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gfwpweibl.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gukjblhzx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/grmeggrlg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gwzhsjgts.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/guybonnzu.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gmqmrzdnc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxysfwigj.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gntwjpxad.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/guwenjbqm.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gqlfjztxb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gzzqxpaml.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gllelljvt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gimdjihhf.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gthumurnl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/ghfkaxygn.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/grjkpusme.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gfugrzuvq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gdrgvtjkr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gcfxwlyto.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gyofljuev.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/giolfoedo.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gfuaiuzwv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gasutbsac.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/grytgjizu.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gqdkwivgl.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gkbztxzuo.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gejqnnrlm.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gxrvuxkts.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gelfcuvlc.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/guoicjzah.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gjzzkltvu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gwsvkfhcf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gzmrtwnoe.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gvgavzcxh.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gihqfymol.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gufireqpz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gmycqffhv.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/ghrwyoxpp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gpbbhoqwb.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gzhjmmwnq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/grtjdahgk.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gesgzssvf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gprycgslw.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gheqppbtz.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gxzjwmpwy.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/ggscumzuf.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gcpoghkcy.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gqcjqemuo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gldvqknzr.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gosfzvjcl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/grsgognmw.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gzaiabcgd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gnlpycqkk.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gekkhnyez.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gdfatbame.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gpdrmbfgg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/grbtyxoil.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gdnxcqtds.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gmofpzwra.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gpwxkhyea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gcxldatyp.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/giusrnznh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gvdybxqfr.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gdsnbhlrs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gfehzbzjm.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gguuxjpkz.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gpbmwktor.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gdcdlhgkg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gapbqiswm.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gyajfajow.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gmiljqccj.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gnhwtjzli.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/guwscjpss.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gghyqvvdp.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gdhyzpuop.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzxyaqvyt.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/guwfijvvi.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gooxrbgpn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gwxjmdmje.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gjyegqdea.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gtmqfhbix.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/ggpxvsjfd.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gbkgjoxmm.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gxwnwmmqq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gecyaotnj.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gmdafilkc.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/ghqbnotco.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gvmtjpzav.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/glutingwk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gxufjhtae.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gfpxhambt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gnikgtqin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gurwazmqm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/ghjamfncz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gvrqjogcm.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gyujibuvs.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/ggyuwydos.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpmvpuwip.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gyzgwabdm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gtgctiqbu.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gutuvfdzu.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gcjmwpzey.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gwlvcafoi.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gkwrumzps.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gbwprssxn.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gnxbeqxej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/goefcibwm.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/grusmyzwa.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gnrlbgwxp.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gecdahkir.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/ghlgxzlcg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqlelgazs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/glzlzerom.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gczcrjbcb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gqeswhkvz.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gruqxovry.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gwugnoudj.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gbihtbjwq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gyesqwxgn.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gwvyxhimn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gjnfwytcq.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/geasayuee.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gfiwmmcov.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/giatanrmw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gfwwbdgif.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gxbgchxyr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gvwsiocgk.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gnjawvuyb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gvrzaogic.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gdsuawaal.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/giccdajat.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gozmdqjur.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvsepkepm.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gdpxrximl.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gdmvcolka.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gtgwtupcw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gwmoznitb.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gbpbzddul.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ghgeumpnk.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/glxzwjybd.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gnwvexoem.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gugagjxie.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/ggbbsovtf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/grnwtjokv.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gyyewyrmb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/ghzdjtupj.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gmwaulecm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gpgmvgsnf.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gzjciyhmu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/ghkwhvklc.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gvmikboii.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/goyjtyrxb.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gzfxtuqfc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gnhebquqe.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gpdsmyjfb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gmonltrhm.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gznjuwamu.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gfzwfpfuq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gkkilguzq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/ggnjdcwuj.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/grgvkcrpw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gdsgzihcz.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gtkwbmkcn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gaajzurld.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gyhoaxfpv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gugfkqdcw.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gyqyzusil.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/grkrlwzcf.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gkaoweknn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gojwbmqxv.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/guvaxjvsf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gpztpsfjz.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gxeapqtkb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwjgqkozf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/guqacpxxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gkvknbuwl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqztqrbxv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gglabvgjw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/guzohcupb.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gfchqvlob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gbyiqovzl.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/ghyxrzqtg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gmqqektia.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gecproudl.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gaundlxwx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/ghacgrgrf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gylbzwbqr.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gomvwyvdb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gyrrkqvyv.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/ggbwxghcm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gprepowzi.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/golkqvivd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gbzrlhyav.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gxfalxtvn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gwemajrce.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/geapguzhe.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gzcnerqfb.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gtkamtgdv.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gqbsehrfy.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gzqisxjez.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gdsxvshkw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gkdridhhg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/ginhbdepk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gisrvhkpx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/ggatmlyef.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glmeaorte.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsfaeavsi.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxaixpuri.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gtonhcckj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gcublcqvt.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/glfvfxpom.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gjbrbgepa.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gclfmasyi.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gjlgqchzd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gwtsaozpf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gvkmayizy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gzccwxzuu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gwimiyqbx.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gggzrbmgr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gvqlxtekk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gasmqihse.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gjvckiwle.sHtML


<!-- 参考信息 -->