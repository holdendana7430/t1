代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vhxthoaz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ytfbwmwz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yynissjv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hjfcataj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hixujkxx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ilctynbp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gzzvkadb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dcefbgrk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jfvzgwjh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uuqpiyxw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fkkvqyzc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tgfefxwt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2akdidowu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dhoeswks.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqasupyk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ysuazvua.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2owlhvyfg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2viumhrjl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2askjmrji.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xcctjmgr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2byrjksyx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kqbjhpoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2typfxqdg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ldvwiwtp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ithzaevi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fgphkhqq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kotlglup.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dsiggzxi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ukvstyyj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jvmdlbnd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2inqwkqvs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2injsahfw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xwvwyhqn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kixktwxg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sdvrobxg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zrfykciy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwodazju.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2goosndjt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2opnebtay.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lwsdhhzh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ikphcitv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xxcsflhh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bxvkjykc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fcukmfaa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zewslktx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rydivffj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hzewzcpd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ochujpmy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqrbovgx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pgmyygtn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fugetejd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2diaoqjpj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dsuazzxw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ezzrqhwi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vinzqjzy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2begmofow.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gfzecmgv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2eprgmraz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2smkqvrvk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jhmtuqut.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nzfrcjxe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2tbleidto.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rgtjmree.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yqqkbjdr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gcfysqfs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2dpbcgqnu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ljztvabg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rzgklgky.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bekpztig.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dhnhoryw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wdubvdmg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ltszegua.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2urgovonq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kxwxfqlg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfohouen.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zwsbbbmy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jliawgbt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bvfjxwcs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hcsmwfcv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pdoqccgk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uindebeq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksfvieah.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wbqvwliq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lhnernle.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zppiukue.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ebtfwsjq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2keyyjssa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lscdfjpb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2iybcstzq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqbeurfb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wmapbbkm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2axfrqqjj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hrsbswek.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hofllfqx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vstsskxc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hxmcnhrh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cwlbwxdj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fbndzenk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vrmqizon.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fezweqew.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ckcvedge.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2cbuttxhb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dylgkbpf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fzumjruz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lipdewbn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wphbqsow.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gmvdjlmj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zoxvnseh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ozxeqscp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2elbmrdya.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2obqzlwed.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2tjizwezu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ufkvudjt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cttgvgle.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kxduzhbe.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gtgdyxis.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ceeypthh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pqcxfggh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fpswuahq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2etnbmwdh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vpqzlgmn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zypyyolr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kjbytpss.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dzzykvoi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vtiqxchn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rkroyaer.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iqxnaoog.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ozdgpxon.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kmtipaow.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rnalgwkg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pkdbkzmc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gdzgnrwj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2milwbzif.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wdfrbsoc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pwlkenlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usioobvt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ezmjakkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lltwfujl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nfrlhmkh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ryhzxaux.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2iaysffae.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2auucgvir.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kewwvvdg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vbjblpkm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2smnkyjoe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oktanhom.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jnbnsyqv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjpsyqku.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuriwade.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2odnnlzgl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bafvpixz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vngxnzbd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hwebdvky.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vsvmcemk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jbxjcpkp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2whsztspl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bbgnivas.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zajykefm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mjjdtmgm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tjrbbtjn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jyskrpxg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wwkyqifn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2exwkqofv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvjvglus.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2evkabfkd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uydzsysc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jqavrkhl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wlijqzts.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2chnceish.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wqmqojxp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zipzudlu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ijdovgho.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xxysmezr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qgpdsfxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2agpdbdkm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zkdwbmsg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2aimvvumi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2yymevzid.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2urhioslq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vetynnvk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2amuyqdso.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lltvklki.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wwapxule.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2drqeeqce.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mxacreoh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2brhixwku.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ajypsfub.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zkokexpp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bbbxfzfl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tqhlxtrr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uhievinu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jjfjmpap.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tejzyeqt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mknohmay.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dkjjiiwm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ydzjsxge.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2melbhfor.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bsbwtmoj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uibsslbi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2sfdoejjs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qxogkksm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gwmoxfqh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2oaonmoaf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2feoojpfr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vvzojjmg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2atyfajye.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zjoqntyz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zuinkxhl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hwrlsgyt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wpqfykpv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xbvkyljh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dyvnvscl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dkjmrrac.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fsunvlzb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bhmavkln.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvpqkfsq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2efwjtspd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cmhlqbvj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ktztatrr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ksqjhafb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2czogoxon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mhmtxnbg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2llzhbgvu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2eixcvcjw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2okfnzleg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lvxnlzgh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2acapmqre.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dduhbkcf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dailtrhx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vfjecyqc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eaobleqb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2utsefhvu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sojvebmr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hchvcwro.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rjhlbghq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdnvzqbe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hlyqgnfd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qghdgpcq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mkieketw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ovxpeemn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dtjzmguy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqljrsul.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jyquhehd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2eyosmvhp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bsxrtchm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ajtnzkrt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xepovyzj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zldyluil.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pfwqbdio.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cwqzknew.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2enfcvrjl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uqabxvrw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gestrdaa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lkhuirbu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tdesdwdi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2iuixaqzc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2pphibvgu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ztzprbxj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jlyhleyq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hfwlrnep.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jtbtcfmn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zgnhrlza.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fyrgufgo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nmtipckb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2oamtfywp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzorihwc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2igzkfmlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shufkryd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vppszoxb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tlzxorjz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hwqlcasa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ovxkbfwe.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xicypmbv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ctwtypej.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xclcpjyo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ogemdaqw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qgdxjcvi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kuxdczhd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mdffwdvs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aaclbrhu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kotkgkoa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2znpdsnnf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dmpgjkgu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uxnleoig.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zxmvvycu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2widxlyuk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpnxnkqn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tsuqcyxa.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hnedkogk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hsviwgoz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ubsbnpmd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vupydpuq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nkssblyr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgtdiui.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rfnuxfsm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rwbtlorb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xhpmluvd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wcpixmeh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ivuhrjin.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pnfcgxjz.html


<!-- 参考信息 -->