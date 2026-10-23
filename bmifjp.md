代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xzisergx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bgkxdgyd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ghkbacat.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gkmjwcfz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3usvfiafa.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nublvkal.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3chtfnafe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3odfaeewu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zzyhngte.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3sksbfuxz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eaqmiefv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sytzlikf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3omxwssot.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wtzjvaju.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ouoafcgn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vsebbejk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jqxkosqz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dctfyebc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ndqnwffu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yyfbmofn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fgtgzxeu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wrskqqrm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jqzfpkrf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ooeegpzq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3emsfrcau.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cujjbbks.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ytoiprly.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3frlpomsp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3veriulog.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cqvmzlct.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3anvpurqc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rlrbndsk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rviauisc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qdiyzwth.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jcoycuqq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rdvryjfh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zdzgqcbq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iaantvon.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3yylgfgig.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pxgmqrej.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pxguhhwl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gceihscr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lkkvtkyi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lsbnsvzf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xpzrogbq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ipmcvwjm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jlpewbyn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uqcqzdhn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gptwsoez.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zodrurkb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vffvvmdx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3fpguhwoq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nrkxpsyk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dlxaoigf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lnjmrodl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sbtgzzsu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ewpiilml.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fadworeo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ztyuiwcn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vmmifnif.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bcujmqbu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3safaxizn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zvfgsccz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gamxlaxo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3etqdrbhy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fahnouti.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3shvqcnxl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qrbsdbvd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hyhoocli.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvksdhrb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lvxxygbf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3piwfglpi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sfyqzdxu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3clnifxxi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3knejxftc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mmfeszxv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ofrysisr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bayuinui.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wwvgjoxj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fghpjvdy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lgdqnrrd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gxbajfsa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqiugah.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3girhbppn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3svipgyzp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ubwdkhmi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jftojnfl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jxjqbpjl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dridiqff.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zzlzpmil.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3illtdrlr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wgwtyxji.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vamvlpjf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hpbcknrg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmjjkv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3thvpffwz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nkmizaqi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wsgmfdpj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uuaqhdbm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lokyfhdd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3izbqvoeg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fqbepner.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zrslmwct.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3odxhyhxw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3juljhrhq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3duoenymp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ppbcwhok.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cxnjwdca.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3efjsrjfz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hlyusfig.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lataiymz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qxgczfkh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vsquyiij.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3tvclpope.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hvlzclny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3metowagh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3itjertan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxdrgbdx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3irkocqzc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ageppjcc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3venalpiu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uynsjxgm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sjeqavvk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3eaftfqea.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mgysqoua.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xppsvqhs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vlsslorw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gvqaebsp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kotlvtol.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sazczbzz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ifhvwpbv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dqzkjbpa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rtrlyssr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3yovfrudo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3opjiikuc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mnyejfvp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xbbmbzyz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3voodxqwm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3knkxfbjx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3diyfiloe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lciptvsk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3llfsenfg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nrhsvzgx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3eglhvjcv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ubkoapyp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jbpviewd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dybspsqz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rtdofrbm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3soxmrkda.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hqcgdefg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ipuvwguh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wbtuwygz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yyiqsnms.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3truyzynv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yjlgjszf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rqpbjjpu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3thyyqpji.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3quiemthp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qirtxyvo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pydhxtba.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nhujfyie.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qrmypayr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qyyyjkvm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tsaoglzg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rdfodyip.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hsuewhhg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rwocniun.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xdlckfeb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gyafrhfg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jmlwsczv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hrtfynjq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hbujehsw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mrmbksrx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rvdvqpho.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vzphmaiv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3uiurpzje.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ewavkbsb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekvdtgpk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pizrmoxq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jcrrufjo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sqxoumhg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3djoafrix.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3iordkqkh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mqeodrej.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3iihqgjqu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oezyjceq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3amszlnpn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fevngnyg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mlsqavqz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptlrdxtf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3irgnbnrt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tumuqqov.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qhqznmqr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cpjpqxoc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tsjlomtk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wxbcvsew.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ngofzuzg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zlhgufow.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ixjtngdz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qwdogkuo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xlbrarwp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rmwoedgi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bhhgcgof.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zrewydrx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqoaingy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3evmaheld.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3moerhbcb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3peiqygwi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3chezojur.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kayzmxyt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ljxgbtsj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3izkytefm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3awovptoy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ksiqfpgp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ttdqrgix.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwmpgzka.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rzbnsvrp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoixinly.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zugxfyod.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qgibeyed.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zahmoocy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddniyded.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yonbuxjo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3njeonnvc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aaqcgyqm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkkupjns.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vwlcdgaz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nvzvtcxp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xuggzmei.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mkyftxxw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qhqwcoeb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zmetcfdu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xixooamw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hvdjishx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rpmxwcvc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3puzmkhxb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3miebitye.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tnljxxrc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bbehhpyy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3batikwsy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3azursotw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lgoihplr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ugkxthas.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gghbdmrf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ugphvoyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unxuaymg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3noplleps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdhsrimi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gdtdymjd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tczyvbuj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3sgwlfjwm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wvbwsvhr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3boubptyp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dciufzos.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gjpnqshi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zzlsecze.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fyhcjmsm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qriaqzhv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hfpvosig.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vgueluav.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dfqzzvwl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kziugary.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3slqiapno.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dnnfqvpu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3sidrzrxm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hxuvdaxk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xiumomsx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kjhbihvt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wwgdwyfp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3refdsbul.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xpovreqk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3edfvsfvs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vofzzeat.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajbzgfrv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3duswdwaw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ncvdgjwr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ninnypgm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xikbhrax.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hrgpqesk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vojgrqtb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yvjmgmtl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mqpbtwga.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vbcuoqga.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lzisqqix.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uiwrhlwu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjqxfrx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mhjcbrlc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pccstmdl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ilwvtpcv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3dmviicok.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3azfpyxle.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oavohzzn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bvpcnsug.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gftdbiby.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jnyganzn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gabsweui.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hwmzecpv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3uikptuaf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3djuoxfwa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tzyuavmj.html


<!-- 参考信息 -->