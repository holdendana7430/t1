代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ykmeddsg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xtnnpauf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ldwplpgp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wsfquhrh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jiznqdtl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wdzsebzr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wmotloqi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lskqubjw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2epyzjzqc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yhpdxiic.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2remqfeop.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kegpcnja.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2soyxvrxl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qkvxrtqq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gtgyiimh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2stfvmgeo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uqnxscyu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wlazypei.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hpfdhwka.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2muhiiyoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yizoxfxk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lkdyrkdj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2njdpwrej.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xvlswbgq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2irskdoto.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vlqmucly.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dsfcvzrp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kovbqovs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wucojtli.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vymaegzb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ebplryhn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2denfbzwu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2iafuoegz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ejydptvl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vvvqdpjl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2tfbirbsj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfadxyyd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2whrdtiki.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hxtliydr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hrzuewvb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ktaedtjp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ymarpysu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gvscefzc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xktwwpgw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yvpelbww.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rrdjaryt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ucdxdchn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zhaetuyc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvtqfjim.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2boiafkum.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jujdpswf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rwiqifgu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2btqsjznl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lfkqabpo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vqyzrkts.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aihqgsgx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2suxsxank.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iswqbchi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cbipdfxy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fwkhpgcy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2laudgtcp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tmgdzyuv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ojakvris.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fypfjbaj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hbxuarzz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rouqampd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bpplyuvf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2siwsqlaa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gmizqsfg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pvzwolpm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2djxhmvgl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dtfxtcgy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2puwbhyek.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2xyyywtfj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dzusfxzp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rlfecpdh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dnrjccao.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ewigakij.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nvtutyzs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rdzpcljm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2aezoyuxe.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2qvidincs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqefnzzr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ystyahht.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2lgklmaix.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gpossxbl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uajdxrjl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mitiuvep.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qjegezwi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2krksclnt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fosdwrzs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2acgjlerq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ryfcfjnn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mvqmfrxm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xbiaefil.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qaubygjn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ynfhuebv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rdzjdozk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vvrbaouh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xeupjvse.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2avdqbbjw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lndisrgi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qhvijwrt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ymbkqlkg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xgrreimv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jpyeyiwt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jvusnwuq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cxalbifm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2degidvyg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2muvlcxts.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2puvpamye.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rmeuppry.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vdwgvcip.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ntognxzw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uyuutoju.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2botjefrl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ilgmegkt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2crntnguc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2utzogksm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ffwduqqw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2aksslcdf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vfdelvkg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdfsedij.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nhifrmqg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2btjcjeeg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcgqmlas.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jttrfzwk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2aqpdllcp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xgqlqcgr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fgkxdrac.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpffjvfn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pmxpkitq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2skgbiwhd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xdfgkosu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2naemchzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnqsfozm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qlhzbfvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gstolhhs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mwiauvfs.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pubkzbpw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2huflgjjb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dbmgnefh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qeewvdpq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2imwbloex.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wnhpxffz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lyplfpsy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rxxlthhe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pugrogqc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2furpifuk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lddoedxd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dsolfwvh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2wplphhkt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qlqxezjv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hriytdgg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fprzlzcr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yynqrtfu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gqlwcohw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2piruahzf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2izjehkob.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2znxoncqd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uftkufxy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xvjylcel.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cfwlopst.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzodqnys.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pvkgguag.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2khmdepar.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zejpwaey.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kljdvmem.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qrawmogb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2racfhetl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hymnjtts.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ampurift.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wnnpzedz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jyfjbbmt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hchgiqak.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmrntjmr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bzjtmdqg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2leqaregy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2midijkgg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zvjbesxi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wiikjknt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fzihcbsm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2phodkcud.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pbqumgbr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cjnzyuib.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mrklehrs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jcfnomwi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mxsxmuok.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2yfcccgbw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lpxfjotz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fmtqjtst.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cnkwswbz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2nyxirjbk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2siufoigb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hrddcyul.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qziadqug.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ovzgmdps.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgleeygk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2djrmlgqj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ylfmhxsl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jxwpkubh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2chvuallo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2erfumwoa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bmbfzvlk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wguingrz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otjyfbjj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ewaiecug.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uqtldvur.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vwmgngcp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pzfivejr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2omftqucw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xxbfsvdt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ekgsxhlv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hyswmqjr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lplurypu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pzkdbwgm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lmmuvybq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cfgbxgab.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tubtfycp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zxdwmsps.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tzdsmuei.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jawzuwmm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bpdtbbnm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kzmcocck.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmjekxww.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2oqbelcpq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmqsnoty.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2swyaiiab.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2omsxdwbl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gkqoiqlj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dwgccfeg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulggmpva.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wlzflqdk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wyakgmhm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lqgpjxko.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qrfckbmu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vwcfmhhg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvzluqr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uggtyzrd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2feemovfr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjfhhhz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fyvniyxt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gencauau.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sgbakshw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qwbrurlx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2szdlijlt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gmcussoc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lgalveot.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzoymgys.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rtaepyqi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2srtpegea.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2avnjwlou.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xbpkffvb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ajeyrgqh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gxaytaqr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2sqgbxugu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2otznlmie.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zoexhutn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2obpitnmn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nondvrtd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2doqgunbw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ppjtsrdy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yamhruup.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cipcunlh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ptnaxfob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orrukshu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xirpwcvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uimrerlg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dpnywpgp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dqbrbuvf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2javnfjgd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ysvcnqlm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ptdcndeh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zylczwgr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rhiezukt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gpxbecpz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pvjcluwr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2upkxrbkr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zhkmbihl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2voaahkri.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2etghppna.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xltvgqhy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mjxqbaii.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cyyomtbc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zkwdmpub.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gqtoyvau.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yjlxzrfv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jiufkpaa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2onkxbcyt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tctrogao.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xfknpucr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dxrjmczg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2csvtfryx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2crvwjpyy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uuiewhtz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ltppsmmy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2mycsasga.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2foubxroo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tmpokotx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2spwzcqel.html


<!-- 参考信息 -->