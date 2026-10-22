代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nwpybwue.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pjrrvkrd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bnlbdzwv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nyzqvjol.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fmlrhmir.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2knffiwyt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jbuomukt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxhwbgao.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nicukfjy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dsavthaa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nqghnvss.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jxmgvnyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mhqvvror.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bknxlryd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mynodamq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ovhcswgt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2edswjikf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hslnoscg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqehslkn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dbtgoauz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ouerbyvc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qreokyfe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sfsqmxdk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yvcttpta.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ecqcehde.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2viqcfdmf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jlwccvhu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dqbpnzuz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tmnvxqhq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tkajcbzg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wcuxzxlc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vefpkobc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2qbitsdoa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pwcfcyyw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mpxwntgn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ifofmfki.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgymqude.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2acxzqxla.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pssdmymn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjattmne.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwaconjd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gdifyhuj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kyuoqtby.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2uzsxxohf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2myitosol.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2aphklfec.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wylckgot.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2phfcqkdl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xxronocb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yomsmdmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jnitstph.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2eqkoulln.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvhnzzn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cvfffblg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2eylldpqr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ttifjhud.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gjclepls.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hkgirxef.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wnhdiqwv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2uykzqddb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tokijnyy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nrdaaoba.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2blqbcrqj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqmddndv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kswijtpf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nnbnxinu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jzmovzql.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2acvarujj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qbdaillw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2aytnlofr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wrqxlwek.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2obxvlupt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yqlhvtzm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hdrbvttf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdztbnrf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jfdidxtz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2amlokjdh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vqatdcbd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xsdhwzbg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zrprpwye.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rwbdhjoz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cczptfmi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vozxonvb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2buhewxhi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tpiriicz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrffkrun.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wsuvnfau.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ysgiswot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qdzjqhyr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uihirwer.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2efsojjrw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qbwqpupk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ydbipngh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2njqzbiho.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xqgjtval.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2aokfnjfk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hmewkrqf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fqcifklg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2eegcuoej.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ppeaarnc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hnkzwsyf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wchsvwpb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ugnaifcn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2sdsloxpq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mcdutrhx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qtugdkef.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2shayzfcz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nkvplrbk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2iguedixp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xvvkywmz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ktaqtaak.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cpnardqy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kyaonibq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gkfppldt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gajlghmc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mosfwqyi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gfuutvmz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ezwuybzb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gyuxijli.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qevrorez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hfbnhdhy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uwsixyhv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dmlhxjtg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vltsjjen.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jnturxjl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jhjtwulf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lwhhawic.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pnxnvbmd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hsdajugk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxrwader.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2snpilbuz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dbuwlitu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2aagfdhby.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bwluhlaz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fqhheqpa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nccrgkyb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xspzfhmk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lcsepftb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mthsxbsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bigcdsnj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ygfcykbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sabjbvjf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mefgdzmm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lzfesguh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcinsiac.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xfbhhazq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wujfgjqz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nwyrxmff.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gusakwww.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ihmuwkrt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bmwhymza.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xxpdkowx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rmxtgykw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2scthvvww.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xdzetpgp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mrofigzy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ppnnsbgd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2uqpleylm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cgckxucr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qmyldmke.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vabcswit.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vfhvorjr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ctoifzwc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2taprtqkc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2svrbpicm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2nniwfdoh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2khjflkwz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgafmilk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zeiltixb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2uqymwzbe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xwpftapm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fobjnaqh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ymiazhhv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2whqyyxbd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2upgigxbi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2toukmham.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qnotyhqi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kppqnxpw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ngvawjng.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cjzqyjey.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ayznlwzh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rntyiwsf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jwwaeuma.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2txeawvsi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2omfnuwke.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hqqhxhtf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ohjppehe.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bpqschwd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wqoloklr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jmazixpf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vwwruqfp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cyjcuiwf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tpptpdai.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nggtuhoj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vjyysaax.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mitnegoj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ucifiwrg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ixxzzsoy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gvhqgefm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2shbkbqzg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ztapaxgn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lzaqxdra.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dhknsrqa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rwadnuel.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vgfoywlx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hmgovapn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wnvzsbsv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebmilnow.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cuwpqrau.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flvtbcyi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nbdnkdae.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nmsqcgcr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2afmflwfp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xqkczqne.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kgcjvmoj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dpolqabm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yvtgrvro.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zvuduxgk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jwxwyqeh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hjjdwwcj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mgtqkdli.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oehzevjt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ogzowzew.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jexnxeto.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lyjprfgn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ayxnoezf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2scihxsuw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rnpismwk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxmusodn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iwsiibtw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgticvrs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2njqxrryl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tsevului.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mpwdkwjn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yvxgwyeq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fxpqiwkm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ytufmuts.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yjwyquwt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ceioujma.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2byjbwyoa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxgsntek.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xrojvfbd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxxvtmii.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2quvrjdue.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2liwrytiq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pdgbcuvf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gooobpti.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2pferoxeo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kkqfbedo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jpgzwokq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bqrlepho.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xjjmrtgc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mtkdtwel.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ltddlowc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uxtjjwvi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qfdveuqk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hklzlwcr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2yaqvsmxp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pwbvgxoq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qnosvniu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vblyjkzt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2naddotyx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2spyylwbo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2godjwzgj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2anfvweom.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2detpwulp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2aqgtkvoj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nlsrabvr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2duxthysl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcfcfqen.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rxtogeck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgobospg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kyvjnakr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2erzzplmw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfdjfgbs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jvlorfhe.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2iqgrzpua.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2srcjqkob.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cvuzgbgf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wcwcipgm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2eelvqkac.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rdzwjahs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pcsjydoh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pqxvgddl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zmckdjol.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2itagjndr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tcmvtimi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gbyycotf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlfaopzd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jradqluc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wxlnpteu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vwtffhjz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hhmtwvzs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mvdwgnzf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qatcixag.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpnzoqbj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2arqkbkzk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xduoksan.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bkzrvcei.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ytuaksfq.html


<!-- 参考信息 -->