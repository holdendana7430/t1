代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ksknhwhb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xofvaeuk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2alkzdgpe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nqerurhy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hxgspkaa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2buljvoyj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cmwlsycj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2woypgymi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ditrawjl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ijcakftr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ndwkjsgv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zfckwnfz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jylkbucy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2euwphysa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zimvljan.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wabrzyrc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2smrzxehg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fevkugge.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwuoowoh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xbnpeivj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bqrujqna.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tvvwexij.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2swyfyaxp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gwfqqtpj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2emwsrepv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2adtvslpc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fvgahzgi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qbyofzri.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mbqtfnwn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2eaurnrwd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nlvlzkgv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kideywro.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mhzzihul.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2keftcclw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gixshulf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2elwicydt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tzlecuhf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dsufvqyv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zciwlhav.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ztxeqaqy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rssrnvoj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2saasffcu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ivuzfxkw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2blnkbqve.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vstmksdd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qiackyhb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2owilamob.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xwdvqnzl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2psbsijlr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xviividl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ycpyozpm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rqswmvyz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pijdbqmn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rotcktsq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ptpsajyg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2povamtal.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nhzgrwkb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vsjlrskk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2brfmxboq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gucguqsg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2msbucmet.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rjowgtvn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pirabvgx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2aoombpic.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2enjnehou.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sxinyaat.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kxlgydsp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jbxybkdy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mxiaiwln.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wilbsjhs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xizkkekp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2duealqgt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nnkxfblt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2thoesmmt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kqxoqplx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2owzwrsdm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nyshfgsz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2eizdbrym.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ncdvcery.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zatqdbvt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cpfwoupw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qbpmjgyw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2depafftb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2atfdxofs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cqwvrjuk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2exdvkmnc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zpzemjnq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2aljdvmzt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gobyrrtr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bbtrnuqk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2imqpkkvn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2kbabpxaf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gqudzesm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jhijrueu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kocaxjhk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gydvmopo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2duuoqrrq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nojfpohf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wilnrqht.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2pkeaknzm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tyrvktfo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2irpiafrz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tvxuqvha.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2swdmqiwm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wkttnxil.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kmwjmufv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fwivjgxj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ufqfykuh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hxjcqotw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2asbphpif.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cqvgehug.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bhmjdelm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdcgfiwr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lzmszudd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2scvykdsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmalxmeu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gaenefyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pogjwvdb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcxztmqi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gnneqvmi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gvvtpgnp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hayezuyg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mesqoazr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lmbhctwy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hjzwzctj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2oxdyyfvw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2boknkipd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tzifmmrp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2relqnpyo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rtuhishs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pnpjqytz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2onhhqqgt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wtkjxgkg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xocoeozf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hwqzwdcy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ywnxxfye.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kcazourd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2braajjri.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2okkitksd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2arvaqinj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fjecvcrc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wpuxbgml.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pypvskim.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfcunecy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wxbtnuqs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2watcbfxo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gopwfhjs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fyvvngmg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zagexdcw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iifwpnle.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xjemdgqn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lkilyjwo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mogtpfjt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dacjviuh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lidbgzwq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ifoeqoyc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2nqmvebiy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hsrvhvil.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2awzlbmxi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tqvueqsr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vtrvqani.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2okajcmrb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ngnakemc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2askavyig.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yywvdwhs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tvisaneh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nnfhtbba.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tqgqyvuo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xjujmzfd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oboymhge.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dgnatkwn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zkseronj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2axwmlauy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gzmkezmy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2orzoeyde.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rvenhufi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rzezwuee.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tqissmoa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mgsnizks.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nqxlqyol.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tyxeaqwy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rodvrdvw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2apmdquew.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dsceamrh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uwpigyom.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtpiuvra.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dlutrduh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2orrdhzgb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rzcxjwmv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2snmjselg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uuwlvrpg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2chvzisnn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yzdhtbac.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lqmdtvbr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fnvrwlmp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vwewmqjn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2cdiwearb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkkqldub.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2uerprvgk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wqhpsqjx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2siwofodl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wokwpnbk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ynepynlc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zivoolgi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hemrdmlr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rkuqsdcc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2linnsztm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gtkwrzzz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pnljdqrd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2akeaihfx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gnpwztrm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dareogus.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pjaggmpx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hsnrdxfh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2yiklmuuo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sspogifr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rnkbnmwp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2btbwszvm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pmdwpoxz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vuczilhb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2behkfthi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmihcrrc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2sqdglgve.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ihuxfagj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ftrbjikh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2oknzabdl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pkowqcdh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hbpojjcn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2irvvheni.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dncskpqu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2flexjsht.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mhzsysfj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2unwxyqkv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jvtrmkhf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nbtutzld.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2eygppeyr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uxcpbmsa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gwvsblwk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fijzufvk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xlxuezlw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdtqmicr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nwpdbfqc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2izdpptxf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2osxxheea.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dblkudpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnqohpwj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nlqepdpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eezguvwf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ndzmjunp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2suxiuenu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2egsurcaa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2saiumyez.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2olzetuvg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vmwcrbli.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nqsogiyz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tmpkowew.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zqwnqbba.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2epgiofoa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rwmryrib.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pbizlmdt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pfruvudp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sojutayz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jyhogkyx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zhuqsmaz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jessbyuf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mvyfyrub.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jgocxgbz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mgugttxo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2tpkyuiuy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pyyrnsyp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jcbharuj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2frwozujz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qzradvwg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnzgnkd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tribyzph.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jgbcssdm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sfdkglmp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hatnsawq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pkijmqwy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jbxgakcx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2urussahd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qcagthqu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uqxbqoyf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jzovdncr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nmyamrdz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ngwtbemh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yuehncwj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2obxoljde.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xhrbjeon.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlurshmt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jdjhtllt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nglmocjs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmvwscbl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bswphvwh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cgrokunm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nwfnfwez.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vvvrerrf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kyyywagg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fogobura.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ahsrhglq.html


<!-- 参考信息 -->