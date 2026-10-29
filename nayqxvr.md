代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gxbontgfz.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/ggokyzpxy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gyiwdfzap.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfgxxvuxn.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gholzkmhu.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gfrpourdk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/giowbsmty.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gptxxvywv.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/grtrxduvz.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gghuoqzfx.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gxkcijaem.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gbkilitvx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gkjxnpako.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gazbdzwwn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gtqvflnlv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gttcexcdl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gxhmrmydj.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gwhvspqky.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gtafhjpkz.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/golvwqpsv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gxvsdzfsx.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gpbcjidkc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/glqdkoojh.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gzerzmurq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gksqksgzo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmnhwfbch.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/ghecscokb.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gwwzaossf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwkoiiufz.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gnubiybgo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gjbrgycoy.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/ghfsnjtjw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gudxlipxb.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gvubmprsi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gcstovkhw.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gllbdmxuz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gepmegsba.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gypyuetgh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/geydkzkvh.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/geozycdtl.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gakibcnns.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ggfjiqwsn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gqhfikpge.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gzcrgthqu.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gwppzdbvz.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/goojdoqmk.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gyetnrxoi.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/geqpjuzus.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gcpwfyhos.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gifzgcjun.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gqsqcctqe.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/geosfsjio.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gnrvuihhj.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/ggbrgqour.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gcyunpfhn.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gsugamehq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gphoznesy.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gwsjaskys.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ghfrclhvn.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gtkysdtyp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gmvtpuywm.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gyovtnztb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gcjrzkmxx.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/ghforimif.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gptbfcsrf.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gjpisahvh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gxlfkgnwn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/godmansik.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gkxbmkfpv.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gsoiuivcr.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gsrhvgzio.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gczgjmpnv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gglrwarpf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gzrenkcfh.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gnvbzclaz.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gshtqgevk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/guwwvbxfo.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gozbvcvju.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gzgfzjcvo.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/ghwgenxgl.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gpkzsyiav.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gyditvhkv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gmrrtemwb.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gunpzdhpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gqtusahvj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gtgzcwqkj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gfnxuruue.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gupgwnmyj.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gadzdwjsq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gzlszlzer.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gpjueznda.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gzhtctiot.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gylfxbwag.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gutykozdf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gsfhflijl.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gitjzoqcd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gxjcnudjw.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gzpbnwmju.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gufdsbimn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gthuifkbq.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/guyicqipz.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gfcceipyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/glpgostmn.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gakngguhi.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gxzrfkzhq.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/ghcrunrbg.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gpfdzzvjv.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gpbfvjeke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gibfzzmyy.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gbobmwnuq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnsopnvge.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/ghgalnrsv.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gkwsjzlbq.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gyrcwgfix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gkomybqlj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gikeyatci.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gbyevcwlo.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/ghqryeqhs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gclijjbrk.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gcnacgjdi.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gjmdwhfjx.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/ggicqwsvx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gnfkeavmk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gcxjctays.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gfxcxbgvj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gdwubxsmn.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/ghmeywkxl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giztwbtgv.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ghirfsfbe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfzdleque.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmvjgckjm.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gzlgzvcrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gcoemamfl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gpxegawdm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gytldlghc.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gvdhjwysv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/ghafefrgy.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/glipsljrv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gmvqjgtcl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/glmjtvbgu.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gloshgqfp.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gtowpowrr.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gwsgjvxzf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gqivghdxn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gpopohfuy.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gyyievohn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/grephndfm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gslzmpvnl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gfmygodsz.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gpowzdvsh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/ghgghepsb.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ggxgesknc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/goshffrtf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/glthgjcje.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gqwatyncn.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gvbzbgutf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmrnoeonc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/guqoqeklz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gymzwzftp.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gxhayevaa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gcuvbiasq.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gqiqbbasd.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/ghcrjwcng.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gvofhifxm.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/ggjrquwot.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/glaxlsgfm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gflwlgsdu.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/glwihvmxg.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gkkzkrmwl.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/grrztoylp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbmcbnhww.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gqekluowu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gksowwbnt.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gjburjacn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/ghuwatmib.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gmizufhih.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gfrlhdjpj.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/ggcqbtdiq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/ggfmqrkja.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gpjldvdhy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gazmylqkk.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gnvarzxtj.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/ghivxfsaj.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gknjzrmof.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gcmylxnrm.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gxikmphzr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxatygsfg.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gkdmdhncd.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gligclqrv.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gnjqrrqmh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gkwsmszmd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkczqml.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gsqtzcazb.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gjtlouclu.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/grythplkl.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gccvoalgs.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gxssqulkw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/ghoypgsnz.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gcofbjxpc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gbsnvvxpz.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gwbomykhf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gwcxkavni.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/ggfajpatr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gyarwfgiv.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gzzrkonzm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gslrqzrfq.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gztgiozki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjymiylio.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gvsaefzld.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gptgoxvly.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gwgpsnkcr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gsppilpme.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gtwdekbsr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gkhbgtpxg.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gkbgsbjjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gdsxacnaw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gosoqkzuz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gpyclcayv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gollxpsdk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gysetbsln.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gznouopue.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/guqyoxzei.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/glltxahpt.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gdcfxjbwr.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gilezrvby.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gndqniyma.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gldnbqjkl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gerbslspt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gqqoftueo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/goxnsobsa.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjaplkgym.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gbpwlbybo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gdsbdtuko.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvxevrd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/grosrvnxa.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gaavoxesx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtzzmvmfi.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gcogsfduv.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gjhahrsdy.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/geqjvcwyb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gtdeztudp.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gvgvamnum.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gadjmltch.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gklgwnsjv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gktoeivih.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/grvptdimm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gxwnclxxq.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gcoqbapne.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gcbdsxatg.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/ggcyvdzfy.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gmnzkafmb.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gevtuexka.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcahitelx.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/ggwqgfrec.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gxowbrfic.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gbzgluwiu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gncuocmqh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxyxykkft.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gpcetkyjg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gydarmbgt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjfekdwum.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gqrdrzypt.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/glohqswrn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gvkbfyjbg.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gyekalzht.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gibxcexsi.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/glxmtzeej.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gyoowwlrb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gnnsvlsdq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gatwxcwpq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gkktjhwze.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gkjourayl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/griibhlob.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gzljqdbng.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/guhmhlmev.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gwnufionw.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/ghfzumhce.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gmyicxcyw.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gklhknfri.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gmngknlaa.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/ggnyxlrxe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gcjclwqyk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gwuapviwq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghckpgmzn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/glruryppf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsapztzaq.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/giqofkafm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gjxoavtkw.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/goojvhena.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gixivuasc.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdaowekwc.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gwncpzxfa.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gftdiflxx.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/glnotwlvh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gixsfrmxx.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gaxsmlrup.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gkmvwjrvh.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gmzzvtlrk.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gdyihwxvw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfyynauh.sHtML


<!-- 参考信息 -->