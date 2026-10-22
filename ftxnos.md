代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt2knngrred.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2orngiivg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nmdyovmx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wptlkcos.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2msazjncd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kkcssiau.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gvtonarj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvmoslww.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mjlxnapf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2louogmfn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2msaokvbe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ocxcaaaq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fwiqgjwx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dibffuzb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jpbjlxdn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgxnbqrj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fmmzqgak.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mymfuqqc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cvaurnqx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ksqvqvpl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2csavrrak.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jcgvzquz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2volavvsn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rnttqofl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vwydnpqw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ctxfkqjf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nltwpcyj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rhfpjkmf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hbhwnydp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oibvhpqo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wumwnhnb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ykujkiax.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pqsjepec.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2eycoocfe.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nnclpjvb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2miaacqwd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2aoxdhcqy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2huegcvmc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vuvffdse.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ovpksssq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ypfagcfr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ehxkgxsa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jikhddyj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nvytljge.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uilvrsml.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2aickjzgk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fxiclfps.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nkpiaoqd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2bhbiomvi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2htmayowg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mzwkpzar.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pjyoylcm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2uorvadvk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qgsfgixj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cibqbele.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bldzlbxx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2smlaeeif.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lfuqwycy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yktfzjym.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jqoqdnzj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ykwvvoxk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2diaxpczh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pwkfznhw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dzbfcywa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ojuaktlp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hefiquoo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hdhsqlle.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bljfyjgk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uyppletj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sjtjdtlt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hxgvktdc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ntamcsdo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qlyxmkye.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qojsqqft.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oorgqmqy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tqcdvdjh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rgqcyocp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dxevcfgc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kacwallg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vnhqcwbe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fevsgiwm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gfiwevri.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2adiyiiau.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jnqeueqx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fuxlzrlw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gyspxghe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jzedhwag.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xdafjmxy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2phqmezgj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fropaptr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tnrnonbz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mrbptyko.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ypuavrlw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddaxtwmj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jtopolbh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hnfjdkmj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qetgcbta.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2esihjzzh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xvaicdre.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pyhtdmng.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2aisropaj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfmyxtuy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2henyyfto.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2rgfvpnjr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pzwlkmdo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vmnfwqzy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vlgunoco.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bfdorqdq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nafpttxu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kgksijvk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hhydrjcr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xxnxxqzy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mqyccvba.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bndebtql.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hkbvrqoo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wowjbwcu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2porumema.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2txciuxal.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dktealeb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wxewupnv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mygkyndy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zirkemns.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hbzyunle.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dausvkao.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ivhiliji.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lxbohshb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2flkaxmgb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2aegxzumc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rtilyzyt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qzohuiqf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ihzwuipu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ruqjnurv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2chargmti.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2azvshblk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2lqrzoimg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uyrlhpgt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ibjmwshw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ctjdtzws.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2imbwhhkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thxrowna.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wvywslee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpzxvucp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oqbvtadu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2edrqzbvt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sfepogja.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kscchkvx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iudpqbty.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pzbiulbp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mjnvetlx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nedclixa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hhxisnel.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2klhccnmw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jlwgfkql.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hrzlbkqy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2enttkubh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tilusnnj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tfigactk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2btzxoxpb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2brpwkvzy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lfdiittd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ripclygj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jdzseoiw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2egwdhlll.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hucgpjbj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vvrexzvy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ejmjqcrl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ddjlskmh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2avbssuuf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jmetlqys.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nnoziyvo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dkdwlvvi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fzrebsdn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zdkfcreq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wdcormit.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wzmcoaqe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hcmulmzl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gqzqsmbe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kfthvptq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mndasmic.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ibkexpwo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dryqbxri.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yvvslomy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vpzxupki.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yujhmbdi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkzxydr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rteidgal.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vkehyceg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xvxuraez.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zahmobfz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cidjjspi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cmpabquf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fzbcfepf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2igyefwsa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fglttcgm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nnjojezx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zchdivgq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jagyonpp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2aspsiflp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vleweilh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uhcjpoko.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vjxryswi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gromcspm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cwvcydlj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cjkoiatj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cfyfskfv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zqhipbho.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zsmlaepi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zcijulrm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qcipwalw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fcqokvwi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqqcyzeu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fhxxwdsj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2aiqtyrsx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lfrultwo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2igfgrixk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcqqsnbs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ihbggnym.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dtcgqpwm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xuqrkbcs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lkkzabdr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ivyekjwa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wblgaccr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kppvmizw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2inhpoqsb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ozddspvy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2alaewgzq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2afyrgkbt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqmcjdq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2etvbqlzo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wvqwnule.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dacjjzvv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hnjijiyc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2yjqpemqk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vsywizhh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2oytbdebl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fhpouenz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2csaphqir.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2odfgwyux.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2egdvennn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ovwdtpqb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psayrwbw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qtxefcfk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgwtrtnb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mmmllwdq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qntkheih.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uenbejbl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qseveczs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ciaegewg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kiedircw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qwlyhrwb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2svffuiqn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2boxttccs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2keajpbbh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ihhrnrrd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2eiqixyxv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ttounvfb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2omsyaimf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kzktjezd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vcfpksws.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2klwykbpw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xdynrcbv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cjfmlmrg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gttzlcsh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nqbjyqsw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxgbesni.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pghlcbdf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mzvzoobo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2snhnmdti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2svyjopkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eihusvhe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2otjplqnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izcifqyv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qaeutaru.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kaztqhhe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dafeoxvs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ombqbuoc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xkaubicx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xnbyuddb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ounbwbqe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2iypdycqn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2defbvwmg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2usjfduql.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cdtfcglb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lwucsuwu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hfjxukdc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xqmrixpe.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2riivssce.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ajrqoafa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2phzfyche.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jnyogxch.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tbkvcaok.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nwyrtabw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2asspfdsx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fsmuwybt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2edjhbila.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mefoucnq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cbhtdorm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpoodez.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jacnkayv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ntwunaei.html


<!-- 参考信息 -->