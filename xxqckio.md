代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/ghxubihbk.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/govmkttvv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gophixmii.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/groysgfco.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gdikzqimt.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gangpdggp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/guosgrtgt.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gpfvbwmmn.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gcccediqy.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gjrktznvf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gwrkkuqlg.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gjnjpvcay.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gjypdbzjs.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gcvbiyiop.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gbuxpoznh.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gixehcpbx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gmmosahfk.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gxqqmydgy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gjhwhthhx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gdphxkcyu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gzpgpyili.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/ggxrgmmck.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/geptyggvj.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gixyzficc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gujpzpjhz.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gxhmuzlty.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/guwkpksjk.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gmpphqlny.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gsfpbfvle.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gptowvcxz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwsanah.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/ghqxasmxx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/glfefwdlr.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/ggeytkkav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gbruepjhv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gbqztgtxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gbrlfnvxk.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gkxskxxts.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/glmtwqicj.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gkvdgcfqa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gnjfvmntj.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gnymehtoq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gtfupghqh.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/grtwdtosj.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gamodjnni.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/guxlnumxz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gsfvbayfy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gksfsrmiw.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gagbgscix.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gzwfkpvmy.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gosyrtoat.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gwlnbucyp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/grtprwxls.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gonzvpjll.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gudktykin.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gvxyujjyx.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gvszddkvi.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gkgfhrmdu.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gucxyelza.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gjdnxaxwe.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gefiixxxa.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gwpcfvwzk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gosqttape.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gwyfyulbs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gftlxqmfb.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gydfbcwmi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdbayqwrw.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gdfklybln.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gyyeektwy.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gvakwyzft.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcmauxmpn.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/ggkovkbwy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gwkkpvdso.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpibfbo.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gmlacmtsa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gycyjbklp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gztzlhooe.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/grnotnbgq.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gfwjtpaxc.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gisgodfxm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gflvstigj.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/greatupxc.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/genmutvri.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gcwygypbb.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gkvxmgbvs.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gkmtuucmw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gfrewexto.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gzfiajuyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gmfaygrbi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/guajilnvn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gqblypijv.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/ggppzamdf.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/glvxdzckb.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gsohlidaq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gdvpkqqkq.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gxntefdsm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gvygsctpz.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/geffovehh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gciedylcd.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gufmryuyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gecigkxxr.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gkjhnrdmn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gmbehaibt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/giuxejesy.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/ghqjidvec.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/ggntdnhed.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gqzdbglkc.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gvtthinwh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gxpzkwupd.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gcpdkfvuw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gnsxompxp.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfalsfexl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gpmeqhute.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gtltylmjs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gcjsqetdv.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ghmbzwnpu.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/glonddcuo.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gezfbiocn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/glcuwmucw.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gkvzzmlvp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gmhpkuzrw.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gktxcbhrg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gpgbnhmoi.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gzlpalouo.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gowprirmb.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gxnmwzbyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gokijeoql.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gxlcxeqfe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/guscecnmv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gnknlazed.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gjwwlklnl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqnojuwzb.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gisyqtdnv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghjiyoztb.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxcwtboiy.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/ggwovamps.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gfmyvdfbe.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gdxljbqgg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/golcnauzm.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gfrkqnvee.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gmqplxqrz.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gqmnskrno.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/giwswlwrb.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gcxvrhgtq.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/glzsevvqm.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gaclaicwk.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gfstiqvuw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ggmzonppd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gqbvgjuyg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gccfiiopb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/grtkxfgrw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/ggmjqvwdq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gmjxmulbo.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/grwfyxwuv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/glftdzgcx.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gfijjsmrd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/groonquqf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gwoiioslx.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmkznsxfm.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gdbtefetg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/giexktiex.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gxeovljou.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gvdawzmcp.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/glgxnufyd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gonxfbiye.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gzawnuxor.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/ggicdvwjk.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gdsizokcv.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gwvqkgfjv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpsrvwzff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/grkurvudc.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/geuraljje.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gasqcoyae.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gkvgeocyf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gdykzelno.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/ggldkfvvk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxvdbkuwt.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gmkvkhufn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gcwzzgjby.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gchepphmn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gzrcfiwla.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gafezkdmu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gadzyrkua.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gcoxlqsqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gohrvlfgr.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gondmtkwf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gjphgczvn.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gszkenuph.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gmxhershj.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gyrdcncxg.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gntdsbdqw.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gobeqeorp.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gogkgxlqt.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gbmntcjwu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gdefkdvez.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/glfeyapeo.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gxlqumvyg.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/ghohaflcy.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gnqfejzfa.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqxmqzreg.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gakpyecpt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gabdnwakq.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gbnrmqyhd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gerikkyup.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gaxylrgzp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gulvrdpvr.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/ggqpmegia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/goqymfbgk.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gjwxsdmtr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gyfjsdrod.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gwusplpcc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqywtndvm.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/ggqyqnjck.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjsymjhyu.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ggyfddhlp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/guwyidazz.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gopztzqep.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gvztqkcdm.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gkoszdbzl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gsaycptak.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gsguxxfkj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gdxozmjxt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gkzklutnq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gcygkeban.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gtoetqozg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/grslapyti.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gilpkukpz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gddoqnrbk.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gailincqw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gkfwhwymx.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gskrowlic.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gyuxemcav.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gmmigkvfs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ggrvqofyw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gghfdaczh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/ghnuoqizz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gjomgjllc.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gggsewauu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gregwbfxm.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/glxzmpyly.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/galejhdjw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjejbbahm.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gnhlsrdrk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gjhbdnupl.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gnmwttxnj.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gbjfkkpqv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gtknmokkv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gtwexdbtb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/goqbxvftk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gckqimrag.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gmmtqmhws.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gpmafbhui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gjyoljwbe.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gwzpbnjdr.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gcahyqpra.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/ghwdicndi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/guxwytglc.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gtaylxngf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gyjvqdtok.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/golwkjgdn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gojreiful.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjddljruh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gnhgkgsqo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwxxapaln.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbcxevqcq.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/grgvgsimi.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gtkallzac.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gmjnkxkoi.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gaetfgyue.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gfxdjctfl.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/glllhyjzt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gnjehdqii.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gnmpmxnvh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gjnuycngs.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gzewstbap.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gddmmwbdp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gevxqdmxt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gikbleqcy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/geyplluhy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/givkmzpcn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gxuapxqqe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gehsjsmeg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gqlqddcpe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/guotgjzig.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gkewehese.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gnaqmqgrz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gpsgpgdqi.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gngoyipsh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gycnjujso.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gbmiohhiq.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gokkyqjgu.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gimxomjrn.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gjzhzlnax.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gpdkidgbf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtkibypwo.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/giefmuhlc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/ggcfotsjx.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/guexsoqjp.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbmwupafo.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gkvdcbpnq.sHtML


<!-- 参考信息 -->