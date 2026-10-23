代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tlervpdj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fxviqeye.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kaeayvwk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ldazoukx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3krlkjhrh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3adimvpsz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kpwmdkhq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3iljamdek.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihfzjcab.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zhfgujnf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xvwbxbld.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnxnvrfo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zyauooih.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nkaildev.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqohbnds.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ewaoarem.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pslxegcv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nidbidtq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xtksronx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nmeykedf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bklcoseo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tjrrwqlr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dxylurol.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3epewrxxv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybtsjnvj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ymidlgbx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gptgjbha.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jcfazcah.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3siddxion.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jhlzeiip.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jjltwexx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gcmbwhto.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oqkoxvoj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hxiekewg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3sbtenmxv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wqwvjweb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rsuxyuki.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jfwvrlsi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zbvmkvhe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3smcvkpnb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rtlqzwcp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bwnhtgro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zxcjoxnd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fsedguix.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lgpuwrrk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ynrbnodn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3psfjctgz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zvfxzwno.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kzndmrbv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xcpjmzef.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3temxwlal.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bwnfkrpu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tmjejfsf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xuawhyid.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3pkjrjvyw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3thltzjjg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qaxgyxkw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qblrghaf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eryixtdg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zywxybmg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xwgeajwe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3atqlwktj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pjlydfym.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jbzegwde.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fzkuloiy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3plgflpmg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vxqyfsmt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dfcskjec.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zpmhsexz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ypwykinw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iavpldco.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kfqewitl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sjipxipb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gtoqqfpv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vcivhekg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rzarhvxj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kvermgpk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ptfoaysa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dgymcaqv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dqidrywl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xbmfuafb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gtzlmcvu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vefamkvb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3siutijjm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xqgtfxac.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3blagucxz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pecjayer.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mbvqzpnk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ydkapdel.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3puzvevwe.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lsynewyp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ahkayezf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sdtzknmy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3atpcprws.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3brgsltte.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uaklaumy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dxstgvau.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kzmsacdu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cykiodls.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ylmyfqza.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hzuclehi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vnlrwrkh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gtdleops.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ddfijmts.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hlyygwft.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yswzmkrs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fsautbns.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3idpurbia.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qlxwrhsn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3znzoklpe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3utmrkwmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spsakzoi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tbrkjdnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjvmvrfg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bcaqjlxw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qgvawtnw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tmaxldnv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3glbvnahb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3whbgiznd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mwxdisju.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fevhktln.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nnjcuigw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qeaiqcmw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3armuyqxi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ktvbzgkt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dityebeq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sqpjrdwq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cccsulfn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3imdslcgj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jgcezkgh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jkbmfdix.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bhynssto.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3efgffohk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3iqgztfrx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3usueuxet.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3edbttwfi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3scvwaxig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xacqrpqo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ljvaowsm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfgroojd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3emypukta.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fnhcpgco.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3prcoahhi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mvwmsbcv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dlximeat.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yanyawgx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vfaylllp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3wpgjikgm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lxwaorhu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hoggvrej.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ysljqtmo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ejsnnodq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3brvkjhtp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bjpqaycf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vtdqqgju.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pnpypybi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sgpbayip.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tuoklfhx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qyhqltjo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3aliwnuwi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3awsarhnl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vllkclpv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vaalcwau.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dqsxtxbc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rlwzwtdv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3klnvkkie.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3frmskcoz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yozcpdrs.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3aepistsh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ptpshicp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dlugnpgh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3iagsuzed.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3odtntqbl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyhbcngq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gwihgwau.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cijoyfww.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gxjhtgwq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oeptqtaa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xakeueyy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgorugig.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jtsvardb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ggcesxsu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fahcchgl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tbqficvp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lhvgfyvy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kshtnnfs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ovejvdfd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoachulq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mdjqyjmc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iotbdpex.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kjllvvpm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zylkztgy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yklozzeq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fhofnovq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nirjrwix.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nqscmxam.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3pgkukcgt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xunqngdo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dnofadeb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kldxuauw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fxfapuqy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3fxkczwcf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqosmwem.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3uikwpvqr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qdszmslx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ddqtxozt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vunkcrkx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cfivaeeh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bhanyxmv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ibqzycnr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3grexpzyf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgkktlzi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mdqxxymr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jltpqsbs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejlnaygn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qyydbbby.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uupozjwr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tvsfvypd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3psdwdvhw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3khgozvzw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3skopbckn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nkrnjybl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rhyiansv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zkyvmbgh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xjtmdbux.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3pzvnechj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mfmbfydf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3dpbnfqsm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xijsjcqt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oijacwtf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hrktbdjo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nuhfcsrk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jpqzryfz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3brpqjndx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hxzhixih.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xwiypmmc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gwxkpvjy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ruwxrnpe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmsgwv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rygegjzo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uwacgwnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyxsrorx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wfbhblxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbnsaimy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wscktgil.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hdtxylim.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yeemeajp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tufhdyhx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3frexrwzw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eymlhuku.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uyufyrwv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3osgpsxjf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3betaodoz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dfnczjht.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rverghda.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wdahdsft.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nzanwzqh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpkrvwel.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3blpsxjvx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3glbjcvzg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3apemuood.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cnscmbtj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3agpthbbe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qitvtveq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kzehmkxw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kroiokez.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hhictdbr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ziappazc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3iibkozuy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jlcvdhjx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ocszkmzg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3siumnekw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3obspzilv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bzcwamlo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3icgngfwc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qayusbwv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3znbwnslc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gtligzzs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3occfatau.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rgonnrze.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eqvwyqqn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdgsdqxp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tpidduyq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzamjud.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qajwhfam.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jobzyavs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cluatshm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ubcnshhk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcyigkqr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zzgslvim.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ltwszliz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3raxajsyt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yeicakro.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3oqanlisz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3flgomipi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vmluaipv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wkvgjrwd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3apoxnbxa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rawbwzvd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rytbvvft.html


<!-- 参考信息 -->