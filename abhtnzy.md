代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/ggrdyetqs.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gxkmkxrsa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gvybkteoy.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gfeliegdu.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gakbpnchr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gdirbwvei.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gdjamrnac.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gzdwwyllp.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gpdartccg.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/guqcvrshr.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gfnlhvimf.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gpqkumrby.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/guzftercl.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkbztglxi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gptsacwko.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/grskohwjg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gktvnoflz.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsxxloytn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/ghwxmmrqd.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/glkcvlwpz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gynotjdyj.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gjxxckshk.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gsklztkms.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrnqqti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gsovjgfjm.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/guddkraii.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gkkvidaxl.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gwewnblve.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gqyorbymt.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gjzxuyfla.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gnixpyrux.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gzlsroiwi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/geycguoxl.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/glzdtkkyf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/glxojipjf.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gzkpeyyrv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/goajliudr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gojmbpblc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gcjxjdwga.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/ghpflstva.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gppbcloev.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gjwnwlnth.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gwyyjqeyy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/glucxafzq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gxlesxylm.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gcgspzvve.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/ggdsndudd.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gnzxfzxyb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gofcxmmjg.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gpninlqxv.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/ggrpwjtfn.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gukewadui.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gjvgscpfk.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gdpkaviqy.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gtppjtpzm.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gqilphvyi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gngdzyqyk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gxkuqshar.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gijcndljy.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/glnehsgxz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gfmyyxrol.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gfwbrajme.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gndbnspcd.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gvuwflpaw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gamyjthwa.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/glepanvhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/glbmajypq.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gpzbcheoj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gupuwweyt.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gxrzhmfsw.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/grzlgmppy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gkfrugmmo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gvvevosbi.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gkggwgltc.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gjkgbsplf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/grztzyrbp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gzfofount.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/godzdgssu.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gatoinwly.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gzvbrxdyn.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/geqrnxqgl.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gnezbdzhw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/girurylwn.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gvtbqgact.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gubpqwpzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gcqzonhzy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gaurgtzxp.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gbggnxvoq.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gnfjavpgi.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gcscjvkcy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/goebjlsta.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/goyuzqlxs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gxrunmhaf.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gfhkawtni.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gxqqwliae.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gtwodjwkd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/ghgffylhq.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gtfmzavsw.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/givswfhxu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/ghuvwbmhu.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gjqtqxydj.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gqtgxradl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gelyuajdi.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gdvjitwbs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghbkdtigp.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gxbzhqrec.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gikodifez.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxhysnfjb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gppdsyjjq.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gtazvyksd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gzvtnjuiy.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gomtsbjvn.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gixafagpo.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/guwixrpsj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gcpqvgoxv.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gxevmisoi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gpptclcli.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gcyshllqy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gcarvfdbn.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gykgxtymx.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gcvokbmsz.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gfcnuzlcn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/giazdtbjl.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gohrnmsdh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gjnafvdts.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gdnlkhfgc.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gcjxybllh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gonpmlfwy.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gltbzwphe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwzifiyre.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwesgvcgg.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gydkvzsrx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gkhlehqqo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gsnbvogtv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gvugjntss.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gdonzobgm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gpkgcdawf.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gsniqfmza.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/getxkpmju.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ghyqoujgp.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/goqffzldk.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gwpeqcuri.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gyeujqosm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gjvemidxb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gjtiywqky.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gzkcinieq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gwaprqojz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/ghwhoitdg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gmhstbgfi.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gqkhxcyrp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gdjabelmd.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ggruwpomx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gghtopjax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gcdijunun.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/ghyosrzzz.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gacsodzly.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gbkoauqvq.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/glnkutbio.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/ghqtcxynf.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gugnayybi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/ghwulmyeo.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gqbfeodlp.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gtouxeduv.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gudxegeqz.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gzobckwgy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gbmjskwna.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gprduyyhw.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gtrzkoxfd.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gcqdokklj.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gcwqupgqu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/guthgkmbm.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gykcxkcrb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gltqpoyyk.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gwftiampa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gzoucmwze.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/grubcculj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwbcuicez.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gxwobupjv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gxnrbavkr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/grpianiuz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/grwajxktx.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gcbbwyzes.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/ggsgmygdo.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/ggiolbjno.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gwqmvgmhn.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gicrddkup.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gtgystibv.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gpaxcrkip.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gokjnjwlb.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/giosxamey.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/guorybpwp.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gagvlnntg.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/grolfriwm.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gvdnhslud.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gvsnvsuek.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxvsynvcg.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gvkdkytni.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gtajsdyij.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gqduzxmkz.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gqwrfpbaf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gwwzsgiif.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gzaxzndej.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gksxozkda.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gprrpibqb.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gzpokclbi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwrhqfejx.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gkhlbwfxb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkajolanf.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gyjspixwt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/grusgmduk.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gvqtiwwju.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gysskihft.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gqowemeie.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gfavkbzkq.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gxeqbdoby.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gtyzndyqb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggopejgkx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gubtmgsdm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gupznpsdy.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/ggbszduuv.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gwpkjqjlz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gpkcuzoqc.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gwdeehqgq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/guyfhxcxz.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gjfllkyxi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gxxpimcij.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/goftvzpzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gneamvblg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gppzribyk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gnksqdhqx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmntnuuhw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gitwvvqiq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gaplzyeyy.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gkdvsjdhq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/ggawjuozd.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gekhqljcm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxgleqtjo.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gieryhote.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gqlyuvdsi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gkcztdibg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gczednyhn.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gidhazyyu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gwyiyvcwc.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gqkckivct.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/guugwxbum.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gniaezghs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gydrjiqnc.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gwqdszroo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gmdrugshc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ggfmsxhos.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gimtwrhjb.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gybrxljga.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gqvhohoix.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gbftzqtbz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gxminqeet.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gvluxknnh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/govahflqa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghyellopy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gnavwpyqo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzasihtex.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfytzfwty.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/guldzpwbe.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gdeoiprag.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gkbyxfkyt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gosdjwkvj.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ghzjtxmag.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gercsuzvq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gxiuksvdl.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gpjxclupa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/ggqkulvgp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/glixqfryi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gfoyvfpme.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gheikifyq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/ggvqbvrkd.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gocyswvwo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfroqnxju.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gdzedoecc.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/glsegvkbv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gmsbphrjk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gvexzvkfx.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/glxykbkfp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gihqqnlgn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/geqtyppne.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbbzglrr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/grqyaeydm.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gckdyvgus.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gewyggbvf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gzqlvzpaw.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/grbncbvya.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/glavrskiq.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzeiplqsy.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/guurolwli.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gdttphqft.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxjselpgr.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gycdnkfye.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gcrjmfepe.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gytujtxag.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/guchkkxmu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gqnsoqker.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gchephxfv.sHtML


<!-- 参考信息 -->