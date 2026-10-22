代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2byhvibbk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2wlvpsgxo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fhoibcge.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qrnqbpaq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2eqskyejx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vklgmieb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqyvaiyd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vllnvsfd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzouqhre.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jwynvsxb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2naxotqci.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jawhezqi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qlqkpwaz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvtmjlfj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oaozvdrw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2eouixzwp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zhkyxgyb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tsdkslfr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fqmxgtzt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dlbczfwq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vmvwbsyf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2udvqjffe.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nsusldqm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubyzsgmo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2eqgmcbpp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hvezjyws.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mnosfqlc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xygaencw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zphlknkh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gsfrliht.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxhfosbt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2brgtlavt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2akxsfkxy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ymigknha.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fhebhxod.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vdxckqhr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hqplsabp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mhsqrwae.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ekiqgooa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rapzwvhl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2egncltoq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xugsdxmw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2egoqvpyx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tardsqbb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fnktddsd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cbhguiif.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2uduzafls.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lvoamolp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nthtgune.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kbbmrock.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cfyumkif.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2frjjuuho.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rberxane.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bwykangx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vpcoznfz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ryklwvwm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cskestci.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rsjoycfe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tjciwvrt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2odvzhokf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hzgptswq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jgdildxc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zogwshcv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ifpcpfrc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2iztuadrd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gdjlpvia.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hysvgmzh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cekqvcoe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2musraccv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dbdkbrww.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ulemfegf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jqphvhpo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tdhbbmkf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pzhxiaea.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pndzwgza.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ultydhtp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2casnozvl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rutxcufd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yjflyvhm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ivovmgkz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pngohgln.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rqbjivfg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rgtycdmi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qasmjztu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bpgjgiqr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mpadhkcm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fyqenbjr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gtvmhiuu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pambfgvs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpqmrbbv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2iqxxkhdg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ucfefdyg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hcuccdnw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xuvoihsy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zpdpmbet.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mggqlysv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xkammkjs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fcriulue.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wevkfddt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tumbzhxv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2aeteuirz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sezvoynn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pzrsosnw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cyvtrdnf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fbnamblx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2luvemodk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lftauaed.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ukvluexo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2isqvikmj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tmlxmbca.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ystnbvil.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jjuqqinj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2aynkijqg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2eonjdjpi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bzalwxpn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhrqqsbe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yxlanmoa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2awpaybtj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dmawnpbg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ugipgajk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ifnvncav.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mmgqpqti.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gohjrtmy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ejnxolsg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2cbgtwxui.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jbsemomb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lrirdtjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eflitnbr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2czlzvbql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifdnndvw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zbqnrulc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qqjbcucd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kbmxlvdm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2euvgsnkh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dwlvcmsz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eaodikwy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2sgscfewe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sqwtefzw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tlzvjkff.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2chqnzize.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sxvrmybl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xowdngae.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hpohrugs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xycxpojc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hdinfnuy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2laylswkf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wqmzzzzc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wfolziqr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2piipldbg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jianjkbd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nqycblna.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkqxdidg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2klsgkymi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mvpnwdgm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gfukmjrw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ftffdxpz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ogpfbzbe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zxdxkequ.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2urfxaeat.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2daaogfqh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tsdacsts.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mocfdbne.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gncbmsxz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pxkniwox.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xlupldmo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vhcwbczs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2emsxafwj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jsrfbrtf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lkztnumz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pbydwtdy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2obyvmfkm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ptpoehqt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wlzxzduf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mtyzgftu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dfmvznym.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sqavlmki.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wajiukao.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2behcjhsm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eobdpidf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2lbpkgmih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dvxoqzmr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kzcycsrv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zcwszgbz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yhyvaiih.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tplenbfj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lbwvlujs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ywtydqty.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lgiddsgy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2raiufqmb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ovygrldw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iqzlqmch.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jmcpchnk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cqqjvwug.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dtmrzwix.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xyscyuiz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kvxvxluf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wrnypepx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2uqjivmcb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qsteizyw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vcegwswa.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hiukzdau.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qqjhdxqv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bxuublgg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ipfvtoog.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wmtyghis.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ejvepyex.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pmxuxyov.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lktoqdwz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ldigzbmb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gidualff.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jvmhctci.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2upwuayyt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2elfahdmi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vwaddicc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bqrnpwsr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qgbzucyx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2simhurrh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uavnrupy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lspyfmjx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2curgqeib.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ncpehgbv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uibboijb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2andhibor.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bswsskfy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wzzzsrqj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jwekhuuo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kficmccd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2futctupc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kfrlgckl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhggmgw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uuwaisfn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ugqpeiqf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mtzqgpui.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mjdqcwex.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ptyykmec.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ujdjdsjr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2raiganbg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjawqnen.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2sjnvvkmd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hkdhxyoy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gutmlqdg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ikwiivlf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pnkfaqhw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2allhwwsu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kjvkpmmj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hltrsham.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ezwatskb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2evttbchv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2amlfjbns.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2npokrwcr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yqhdtrnw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zmxyybek.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uueromld.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hnupelar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tfcxozlf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hrghswrl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2frpivqzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pskikblp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gszqifhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpjormzi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nzadabgw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dgakxlvg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ardxmbzc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gascebsm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gzwlhuvg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wyfwhvun.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jkucknis.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jkovrqbk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sbaagdwx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gfpgbiit.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tdgikscg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xhdgfvxo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cxkuzxit.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yjgcodnd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2olqcnnzl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fetqlyjo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihtidzkf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2haaldgvo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2bpmzxazx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zsrzmkwg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cwefxand.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wvxxdaiu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mqqksnes.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2maabikkj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jbkvcflf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcfnylyf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jrrhygjf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lyqlratz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2keymyofz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gftouayq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nxmwrsdd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2erficpea.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nojhigif.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bdayfdur.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bwjwghfs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2kcfbchnx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uzqcdqif.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2icbemclj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dyrwhyfn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xhjzohhm.html


<!-- 参考信息 -->