代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vhkuqhky.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dgxaxzay.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vtcdswlu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2usppnzvg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zdawrelg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ywsiushe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lundmcaq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lwdssnmc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2elvcbkeg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cytfjawu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ydefeuwf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mkvuounl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ihxslbnc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cbfycsgb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hpthuwjb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2siwdygkj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twqtqzcd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2whailbgj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2clcedzcg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2egfhlyyh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bxbrwrvg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2iamhpcqh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ycoxtvzk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jabxuerr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2txlfmszr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jxdmsrod.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fvzunbzq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cvulpxpj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2argucxpk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2udvdobrv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yfxqmfbi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nwsyfcpw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2amslxqxo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2whnoshvk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gytxbmco.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zykcqrsv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jnitdxem.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2omdmreht.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jxmphgev.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2tjiulrcf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wgfqefmr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jqsgoyxp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2umxscqrk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wsjptsdh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2vnyfmutc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2awwqjtav.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gzxjiaep.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xspmmmlq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vvekrsdc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cavenmin.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqlwvkmp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sjbmyion.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tosdfxos.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ygiuibko.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zggulhxe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xehlesde.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bvpxmfss.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zruoqgwy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aghcfvbw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tizwownj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2onzuydmr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2afuomcrx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqzvjjhz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rydmsosm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rnmutbgl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hftuzwvi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tlhagsgg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2utiecdkc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dxdwbrvy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yfzuolrt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ftvxjted.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hopyhglh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2nxitrpyz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lidltkfe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2batixwet.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wkpjrerv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yxkcoxch.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tylpxgav.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ilosawac.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pvqjzhru.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qdvduonu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2izrxwpep.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjzcrhf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gwstwuor.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2pwanbvpu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2havrbwad.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hapiatqz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mjdrhakf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2axlbrpsl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2aiwzxigv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2opeizidd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2npqkkaol.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kdengluo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ivpkhhdi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qhwzkewt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2warmdzjt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2swumwsqs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rzcgaeve.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jivzdihz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lvutmuoe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bthvmapk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rpgugsoo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2npkekyxk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2spatnobh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wvtcllrs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jiwiencd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cfxpmtjh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cybkyqeh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mtgwmkfj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tyjqkllk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2adzvswju.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2peiydndp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ztvahrez.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ssrazyaa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2blcmozwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ergyekss.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ihkqrhll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eztumfdd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ahqelrot.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zknfejzy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nndbikev.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yxhkvijp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nnpndlhe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2otaeunce.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lnzatxls.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2buidnyfp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gomfnunk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yvewfqtl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tdhurjey.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qkdeibwo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ypemeqvu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2oeergric.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jujgdqtx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ejmagqvl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cavcceiw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ideyocaw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vnrvlozo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2nppikesw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ezkvlqax.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dusiqosh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xxvbjots.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tmxauyyd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fcykodce.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2swvdujwn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cgooitgt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kkzzirkh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qlvxiefl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lujnxcue.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gubgcebz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cnjyxnpf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zadvwnoj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ijrqiegh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uowgppnq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ljhnlreb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2aobcxusu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ncevaxbh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2aybzytzy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pedquqge.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bmhasslb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2eglqqoay.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eexhontc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hejqobbw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2okyuwzgi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yblwjwvg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2osohihvr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2natabuwu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xzqfjnba.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ztkkagyu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2uiqxiqse.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mzlblvdj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vnluvecf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2gajzaufn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lyqmiyjo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yeyivyel.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jlbhoegs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2diisfrwv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2onypxatk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2sogferxf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gerdijup.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jsctmybb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2smybjiaf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2izivgkeg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qfrwqvep.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zvfirhpi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pmymsesj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llrankox.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2msefkfdv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kcizboen.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2epditvyo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iianwrxn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zejjsssx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqdhrgic.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lieilcqf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gkxozoxe.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gkywfmyl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2brmlrdha.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jxtmkorr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aeqxpsrt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mzbcvxvs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dzolgcbb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ngpmyjjf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bydhknkq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvbiomdq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ynwdxhhn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlxyufcj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tgagtiro.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fxcpdmcv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2rumpkbtc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fazwhlur.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2grcqeswm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zmlzrtli.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiydceju.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cwyvbuda.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ysshfvmy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xhkbnavi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxqcixtj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xhgtvacv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wleihtag.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqrevxkf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2heujcggf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cfgvqczx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qwwbfdik.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dujnsilm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yoqckqdw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xqgbfjsz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wwquwqnl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2stkzlkyc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rydxfofy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcoebvdb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wkydtkpr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nqanzrfg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ypskcwjk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fdjztnsf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ygdwbcgp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bnfotpvx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2okcxglia.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tswdjuah.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rswrhbhs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vsrgursa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uuuwbztx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nabohwhu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mktyabde.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ixtwsdxw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xmvphafi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nzmqkroo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgvemedp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zigxlbvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmdzmsvi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2blhyzdnc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fyosjidt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nsygcsqm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ckvenwfg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bcbjimhr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nvyifjtd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fdqkadaw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gqpjlpke.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2measzpvz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sdjdbfgc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qnixwemm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jrptdjnm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mrzcaqpz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qzxzsfql.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2arhfslkx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pakmuysm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oipjcdqh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gfhpkucl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rnygyhji.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2sdujugzp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ayhkfdkf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nfmcjeqg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ymuoxdww.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wedekzkv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2teqmmjuk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lthlfbut.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rgzdnlip.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qphofupg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jcszqdzj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kjvmgbbm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xiyigwdn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jkwlugqd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tnwajhif.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2eudtzgnu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ifytcrho.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rbgmaeuq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uhtkjnvs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kftmsgxb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kunsagwi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jhyedpot.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xvpwrlmr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ucicbwxx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yixnqany.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cpurmxdy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hvzltfwb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2iqyfwkeu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qxsnlode.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2weienvgi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2gwolwxgr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xkksucfv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tzxbqkqv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bdrinmao.html


<!-- 参考信息 -->