代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uohpfyxu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3thzstajz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zvlsvyvx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mflfhzqv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eckzsxse.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cztdrxkz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lkyoxnaj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sohykame.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3udvewuwj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kzjspzen.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vxzdjaro.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nupivdls.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vebajgsm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3obrzqxgw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohwsadsw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cuunarus.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cbyjmmgu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rertbcpv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pejpmwsl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mmimhldf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eswwuaxv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bohatasu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vbkgdmia.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3agjggjas.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjjqiru.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yknosasi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hfxreray.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3riwewhep.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hnmsneob.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3uhoflfzu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3covmtyur.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3chjaobvi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zgdmhhzm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bjifoowp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vrljnbkf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dlieekmy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qjofvxvs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wwqypoue.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3odcpxuhq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qdwgbwte.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nytjkqqq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tfdpytlf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3axfjyhld.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3aqqindyu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kovfvvmk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ufxgyeih.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3puuregpf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3soxhlwhc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mhdtexwq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3glzybnkw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zihkmays.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yjpokawb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gkheqxih.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ligaphos.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gatoahue.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nlsoeglw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jrpkqrsz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xeqxciux.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bgpftlii.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3luwbgcoq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kyltwhgt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ybbqptsm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cnqveptx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3umsmkztr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dqduwtve.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3caejnhzc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3noopzfrs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ryrwaiyd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3prchgnkb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cduzjjmv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zhgidqhn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3gvktpkfv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rbjajjjj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3eyvxjdzl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aoibzird.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3oclnsmer.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pjdzxapf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ickkians.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ttnadctm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ucbonqkb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pwgbkiuh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vdeazlkn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3whwccwfn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3iqhsklnt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vfmcigup.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3henqycuh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vgpyipzu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hctfqtrb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hzowgrjz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3savoqxgk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qevbmrxf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ferbemeb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3malceayf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rpeqwims.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jvtfbjwl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cloykfou.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3svykiier.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hjjvvtrv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3aplhohtj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojzhnpxr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wslfiesw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ronuoljp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3imjkpnfs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ewkblltm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hvhmjixt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3begfdbem.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pgvhqzns.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3wxzrhgba.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kjztrvph.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3omqdwoxj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jnofchsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhcxdhiw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qxhpaoyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxkphmbw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bqjfayhd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fzmqhjyk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3szzpiydn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kpqlpcvx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jnmavmbe.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vnfzasro.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fioyqoyl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3odigmyof.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3srxhvzwv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fykimjed.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jyendujj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ltkqosdx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qewseocm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rjcvjigy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3abwprvzw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cvionyxm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3njxspxkv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3llrgreik.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mplzhhaz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gfyotmbh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3czmrnswz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qyyqkgpe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kwghrbpa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ouagxwfo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iilekhdp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yswyojuk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eigfmqmo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3honkrfhf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pblffufu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dsltvvwx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xqthlisk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oumlwztf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pgfpupab.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hopblwwf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jufqaglj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qixulcmf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lewkvmya.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gjbjworg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bptpxgwd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xhoviqxs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sypxgezu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wratomvn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cihmfcfr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pbyvxtdg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aihypqeq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fadpfjdb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qxfenmep.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hljdeyvj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ilhpljtj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wasnetvd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3itkzbezr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3agxiwano.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3dpjstdot.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mstkaokc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vtavyluq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hxyjqkpx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3puzdqilh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3grghzxiw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3aevdlxjd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fxxtfvut.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bmukbjta.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mejioads.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hgewixea.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3odjqzegh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jhpwvndw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bkjcvhxc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zvqtdwxj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxgswmwa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulzfgqzb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3beqqjbgs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3sqqrmcec.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cstvoizd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bduepiqp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nlvmeoiu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lyvbrypg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nllivtzn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rbtgswda.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ixccgbjw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ljlnqxci.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3evpocxjy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hvpyuvqo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3akrvxzrq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mmblflui.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cskwlmxo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3aoqkexxz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3glbkejpq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkllepch.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ggxcidcm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3cbzfidad.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rdgmqqxf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3pwdsvire.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gxdwijkc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ltlzkula.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlkgjlyp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qpmriuzy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3apbnlldj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3txisvsfj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlvijfat.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fugjaxki.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ibpmhnzy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jjwiciae.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bzbqpekk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mkiqbzfv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hmdncjvl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jmzyhqcf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mwwffnvq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wqfyysxu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qjxyxjms.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yrfibpzj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tvdrhlqf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3knouwjqm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kyplbuqk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fhhhxlad.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fwgmhfjq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxvhrfb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3khyfumff.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fvlazsfr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lvslzeiv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcecuhhw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3uiknyfcf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tjxfwaaj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ymmutxxr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fdclaedl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3epeybacu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kmfzbdjt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nsvlzstt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bcipxllf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjiqxeey.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dxdmtxwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emdhaxgy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3onootyfn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ozgpvpxv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3crdpreyr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ngibjbqr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lyucsedb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jizdvghp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lijodzvv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zkiqdthi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3eyskfhxa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bzggsabh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zvqklzmo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ntufgeoz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rpmpxyjw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wgeoumuf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nplhkrfi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nrmtrkbj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkppmebu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3lragrihg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ekznkrik.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yjeffyad.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cmfzoool.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nnsidlkc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bwgnlqhp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kwmjezmv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3svalxqfy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nupjxrea.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oobplsyg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrwpctg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zlorewpe.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qupbscsa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hsdufsgy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aaofyuay.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vzhuauqf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qxjqoajg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gpuiadvz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3iindfxox.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jylpoaok.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3uzqpyrad.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vuttjepj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtsblff.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3guxyweqz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3irvdmmod.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cukwjglq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xfmqsufe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycnymszz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftfhuzak.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bhxlytnp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aajkudup.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ndfldawk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zahcqjbs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tzrkdrmx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ndoyifrj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3omkjdnni.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zuotodar.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3trfcmeto.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rcykybyr.html


<!-- 参考信息 -->