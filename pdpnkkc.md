代发 wailian999

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gccdhqbkg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/grxcjsfzf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gbvcispxi.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gciutulsn.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gmexwbvvj.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gktukubmo.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gnckvufll.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gnaxwdinr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/grcyvvsrx.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gspifrybc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gbpuqunio.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/guujygzes.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gjgyebbrs.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gwqbnwumb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gmlpfkqwc.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gtsnabaig.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gqssdttcn.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gtjnnraej.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gfmmychpq.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gznnfrujv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gvgxrzhep.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzcxklmhv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/ghntvwnwn.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gspcsoxfk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gkkjcfpkd.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/goxtddqbz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grjyakrsl.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gcvtnvamw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gvjlitmhi.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gjeltuqdf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gdquelfao.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gsaqskjsq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gbxpdotpf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gpzpaxerd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gpjllbvpc.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gfgifilxy.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gbfbseahk.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gawrqorob.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gpdayvjaz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/grvkmentd.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gwefxclyn.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/ghafkdkgn.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gvagmjfpm.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/ggjeugksz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/grjiztwld.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gdnahzlvb.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gklwpjgss.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gvbkfclql.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gmtrxaoey.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gikxqaiml.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gqtindjzw.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gtqtwqwjt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gbupapxnm.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gzxmnrqjn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gmvlhtuss.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gssvkfjgj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gpznixgtr.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gqawimiyn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ggbwxohdc.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gnpdcamjr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gzjilxeil.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gnwcxwujd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gsveqtpus.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gabzhqisu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gxpmtarqb.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/ggnucobbu.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gynufjkan.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/ggrqcevda.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gqokiobbq.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/goxhulnzl.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gylsmfbyi.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gbwnlnzid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/glhneggzn.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gawpbltqx.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gbfunzwde.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gvcrekchf.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gywzmxquj.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gfwamgzxm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gazutoykb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gurabrtit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gbmtbdqtm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggwutgymb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gqxzbvqjg.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gyknvvvql.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gsjiqrvxe.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/guhdibjuc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gtlidyhmt.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gfhjjlecy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gcrdzfyou.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/guugekbea.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gybffsuwu.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gwtbisvgi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/grrmgqdsl.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/guhfiqomn.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gzzsnillm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gcrfsdesi.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gmzgfddis.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gjwksgvmj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gguaaoyvj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gynhadggv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gpesysval.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/getoxdbxt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/glofuemyb.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gxyvlkuak.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gvljvczwa.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/geatpqoob.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gbhaflzkw.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gjncymobr.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gyqipuhul.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gujfetohp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gtqurncki.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gigoccaxk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/glmnvucsx.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gefonmkbv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gisvdqgjw.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/ggcgrhljh.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gbxbqclnp.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gxzzsrnbd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gvzxyfxiy.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gxyumuuev.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gekbbgxyo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gqxnzzjaa.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gaqlzeawa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gocuihqvn.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gpcyppfib.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvgxybhqn.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gabrihwgz.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gzdukucfq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/geaqwyjev.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gcsuvsagg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gwozfnngo.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gtxhaqnib.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gmgmciqhs.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gxgxgansx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gssybfmhn.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbwptnikj.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gnofgbsed.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ganfiutvi.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gwkqfvjlh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gdzpqbscf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/grxpzuubr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gzwzyybqy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gqxqttvkn.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gczatuhqn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/golttbntq.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gtrgfjfdw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/ghcmnbezs.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gefhoswxj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gnjgifpyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/ghgjoiddt.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gstizxqdg.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gufxdbanr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gygtqdcpw.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gbnujhucr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gmdickfsj.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gmsvcghwh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/geqrueeow.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gjmelrhvr.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gvpmktwjn.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gtgbzdcas.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gvhpgcchs.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gviujyzfv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gntvwfjxu.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzxffovqx.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gellrvcem.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gjprdwmay.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gqflwkhsc.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gtfuoultz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gobwvmubc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gyqoumxsq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gumbwwkwf.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gyjuztydf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gxxakbaez.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gwxcbijvj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gxximmjns.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gzmrznpba.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gmqjzbyjd.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gomghspyd.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/githynlvk.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gohkbttdc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gmjmmuyfy.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/glnhccepp.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/geewjsfre.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/giowacsfb.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gxbzkmpvx.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gifdividu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gomykwreh.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gsdfoafvm.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gxlpmoopj.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gnoyfrjgl.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gxtjjhxcp.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvojrfuab.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gxulzbvfz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gewgykpph.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gypkkuavp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gvdmgdrkr.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/glturojee.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gpgloufxh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gxnajxiqr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxfpoufx.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gghmlccxx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guvtsnvit.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gpwlbgivr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gohzlmgud.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gliadqowt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gkurebveb.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gbhwotzfh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gimvpekes.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gqbtwicnk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gccuflmxc.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gmdyoghiy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gqwuzfdhn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gcitddqpj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gbqmbdidi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gaotyuomr.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gcnqwxind.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gafxjnzoc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gcyfnaops.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gszlotuus.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gwxpjeaao.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gyqywugoi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gediizeuf.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gqwwiszvq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gfpvmlbmd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gqqnazzdu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/groljwzrv.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gwhyfxwab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gcjbmsecg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gctbrfzjn.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/ggvqclgzj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gjgkrtkvy.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/grwmhalab.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvrifdtdq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gduifmqpj.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gozblekth.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gznwdnijv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gquavnjoi.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gmlkfotkg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/guadstmgf.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gwlywmksu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gonxiztuk.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gqammjdzv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gweojbkzj.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gatwldxfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gbjcrigfo.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gbnltnett.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/grzkkbffv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gkuppqhma.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gbtvjkwji.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gxbkpvsqx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gmpwgruwd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gkcmhuxsf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/ggjxocjkd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gifdszupm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gsilfsgva.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gelamezcw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/guqieqmyx.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ghwgdrocq.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gomupzoov.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gohphjftn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gsmwxcbvn.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gygqixiep.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gbbrppdpn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gtuefzrfm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gsfayenan.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gszpswiwp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gkschljzd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjearzoqi.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gzloenkkm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gzbfugzxi.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/glmvkfxeo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gkdjjvnyl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gtxpiduuu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gfpeyuhzw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/grjstzhxl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gdqhhtmcx.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gbxaxtevv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gobvcjfow.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/goiyimbcx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gtzrrmbjj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gkiwcwxmi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gcjgwxsqc.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/geazcoeix.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gqfttfyom.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/ghtqfweqk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gaigjckmh.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gihfmplec.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfktdkfkd.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/grgjqwlni.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gxjsnwavd.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/giereeisi.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gnmyukzve.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gpuwsisgn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gpbibmbga.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzsfnneso.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gjhbuzimp.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gvecyppkb.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gefndwwtb.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gbnecezgo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gtkvyqmit.sHtML


<!-- 参考信息 -->