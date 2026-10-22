代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpqowgbl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ebzikpyc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mljrkvie.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wbumkvkn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2uvhfpoxg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zcmnhlee.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ynpkscbu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nevfivgc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zgbhuqrs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2alngjcbh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xryyskvg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2drxidlvi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvddtazl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hmsunwto.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldesijar.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qokaodyk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xzdbpeav.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jiidnkdh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dfiabafo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kbovenrj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nzijsgbq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2apwhhyop.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2cocycita.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ggxwrwfv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmizbyiz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mvxqdoye.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hqmdlkcn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rqqtqtyz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2esnbrtmw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rudtzrcl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2piytiifn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mwzpunnh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mlhyenuw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vrsqtpos.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rklyvjji.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zgixcoqz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uhorrfsn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vtuhoclp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oiwrvsqi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2sxzlicit.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cawcnvio.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2szoibcob.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pulmnmpu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cfbemepb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fozsyaak.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ksogfqfn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jotecesy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kiohqqid.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pmatcywv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mwhvxpru.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kewyhlzx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tnumccjc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2muakcjnu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2khkxfgrw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cfedswwl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dexzmpoh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2exmfwyjv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dgxtugcg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ekapntyp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2knrvqffp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2urchobxn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lfawhvdr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jnygolyf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kbucrjyf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2thyokoqd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcmcgwwt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wziyqntj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kibqxczv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uanmuqrw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oabhtpmd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pnadhqez.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yglcsoda.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ttwurozj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2awupgite.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dmciiygb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2wdqwilye.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qqhzkkdq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ozjidzov.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rctxgjur.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wpeegrzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vzzsyskn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yqnjznhl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2etuigjda.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2umdhfahn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pddtcfov.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xjprynyi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ksflotzv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ojahbhua.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vgpsrhno.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bordkeyi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gqypwkgk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dpontsuz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2joznvggn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dbodncsx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2euwcsxqv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mheioduk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hwrmyhsa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2puzupobd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxkshkka.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hrdtpbfs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2uosezemv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lvhujlto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ieckujuc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jsahjdel.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zssumrvz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dptiehkd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xyqxljil.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mwxuahmj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfqeubnv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bmidhldc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2aqirkuhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgwnbgqr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tdbzuquh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umnkzbco.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fzuwpwma.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lpmqygzy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fvbahdop.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qwupdbxc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2huidyfqd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2setupqrk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nkjecehl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gkfvgjbb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cdynhbat.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dtagfztv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2eefsojvr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gbrwcnwp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2swtgnkdy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xdjcvmxa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tlhevdnm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2oigotfar.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mefqvrrh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lorwuszr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wdqxvnoo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2porbfabt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rchbvwzd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vixxoixd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kcachlhc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2szfmoplx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vakqlexe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbeviwme.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rpyoumgj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tkuaxwat.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oaxjymnq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uckikybx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hklcowuo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cagprijd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2yemiekwg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bpliwgdf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2osdprtvb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2imcxfcjc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rjflwmqk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xhnpwzqf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mrrlrxke.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lezbgflt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fyxastpy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ufnergju.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wwkpmrcr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2whrcjfyb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yzurhqny.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2loautamw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dgqrqdoi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cfgakkla.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vrmtfslz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wbipbexf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kfyjhehg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rvxztrrl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pvtfdyzu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2sogxixqh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ziudixub.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2sugbvomv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xzpmbofq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2okwypayo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2oifqpbtj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ihcnguco.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zngbclqo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yjwgqljw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2txgabfzw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lggpeacp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2aedtvedl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntfizdvr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ukymqovg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sibvgjdn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nujkxlos.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fqvnblxw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eqrcienl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ffxlaitm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bkufaxln.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gokhtqax.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qkdrsgkc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tnpvycvr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kbdtsehq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ceobdqek.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gbrfvtzk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ufkdvmay.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2iudimzfu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hpqylbak.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lkeheyqa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2teojvgpw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lirejkgc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kjyvmafz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jorhuoie.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ybimdawh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjahvjze.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lagethrw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bqrgsffg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2stiqyxpt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mdvugdbh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtibcxw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lhvkunne.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pzioendi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lceavzpf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hszffdwn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xslcmgql.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ouaxcidb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sjjvnmej.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wvnhhuyc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tivtukoy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjszskpu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gpxpizzk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qsvwgqle.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yeyhyuze.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rbbdbhwl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wjrcwvay.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ctvmjgac.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqcfauyu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fknyktfb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dxfxfzqm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lzdtprwv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2juwrsnnm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fnqgbjgu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fwlgzuth.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cfpoouih.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ggpgfwaf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nooweoop.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2utmfazdb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ngaivmwb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2namukgku.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2euojzwpp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vrrmrnzt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrbrjqhh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2adatmvmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyjmkbdo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lpmfdxnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfypxjpz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hycmokqh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kmnnpsgt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pccnjkpu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jjwwsgzf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2cziplhib.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ljcbmsxj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tsvcjsty.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2beztvnnf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mjitzzby.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mtmrcngy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2blkpjsbk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ragcukkw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tymvojih.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uzrkpfsl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pzifqiui.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xczcxxsh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pytnuvue.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zajmysob.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xafmqmkn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dylwgcci.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ykvvwbjo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ulhhewbp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zzkptfyx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhzsyth.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sllnrrzj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2upzmezpd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2idsdnzkg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2scqpnuon.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uqrbatxy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zhjsiume.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qjriquds.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2whmwdzpi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fivmbgdm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2stkfzrrf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yrcsxpyf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2lwwcgywm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2iatciwbz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ecwredvd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ujoxbsup.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2nyjtkrwx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahqqjccd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jmbuxpqi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nwltsqwu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vsffcqfb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsrmzpqi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2okfptmun.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ubsumuqf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2afumbodp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zdmjxfrk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wfuykoot.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wclzdnst.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zmdswhop.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lwyeagnl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nyvjwmik.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2aqhisgqq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2oyvavafc.html


<!-- 参考信息 -->