代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3alisodhk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ivkdiejg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3iuqycrve.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bskhirti.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wkpatrkz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3paolrspv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fekunnqm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fvkmuhsn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvpxgrns.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pvruzvch.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gdyivndw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ztsnlrad.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjztvcrs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3provxepk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbjmvfiu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3stklkxvq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ghvqamfx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xbljtlxh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3olkflgbm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3myznqetx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vpfelcwa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3drbmysdf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kgvycaxn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lqdmfece.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wzxnyokk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zgutlgul.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3eforsbdl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lkvqxbzj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hqdzscgo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3zllplwbs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yttgbwxi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tcjqhibk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hzqnnwnw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3axnjkkgp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kjfcyuyb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3odlnaesu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3acrpkcpa.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kgvoxtxk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cnrazrkx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gkczrqug.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3uulrjzqd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cymqkqrn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bbypmckw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zuvbnnpe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dfdhysmp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3piuvaugu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nfgxegss.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3khbzcpzw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jlzuyepa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tbpfzfhn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gpknxgbn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xgsuybvf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fvgtedhs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jrymnaey.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bkptpils.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zamwqxdb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wjrqltvw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dosgzodt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sfqxzrkx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3spxrnmhf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3iyxiejtl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cjalteue.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qigujfmv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zvzheiwy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mtqymvox.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhnvbwwk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3oawscgym.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bcldczhg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bhuthhmr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rsuayema.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3soxzciep.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3uwzsgqdj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zlslzuti.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3utudjavi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vqaraqth.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gxlnkwsd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ojisujts.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cecfeagc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdrjghi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zmwakncn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3edsrumac.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jzupivam.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3izkgldnp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pzbrfngh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nordqhvc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vfaedaws.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rnaqhwvc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cmcyqpqy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hwpbtcly.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ozcmztqb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hgncgiqc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nslcisxt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3eoqutoem.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3byyarlgv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iyanzvbq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bfpevkld.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3igumoauj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dndawvuw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wgftgjdw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tkhgonrt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3aihvcviq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3trjmtplq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oafppbju.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qxwovzrb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rotturlg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3imtclqie.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wwaejmzy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sveudfjp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3borsokbn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ovjuxmcj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nmzuhhet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iovrmhua.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mauyiqta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbgxczqo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3piynltct.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pshdligr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nctyegca.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sylqpoxf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pndhkdyb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bldermdx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xspagrmo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3avpmiqie.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3avquxenb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ybfkvish.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnahrvre.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hhcbbcny.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mishyktn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ywgyuqeo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3emqwrylm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zkecliim.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3antawodf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lxbipiyf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bbxrhkrs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zfifnpvs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rnqsxpnk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxvpecoe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3uouzuuye.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3diicoobo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tzvaadsx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oehikxly.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ihizmyra.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zneqmbuq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3isuevody.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zaactfsn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qnbapvid.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zfsbgmiy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sghkpvyv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lartnuwe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmeqzenk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3forlbyht.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kagmpeky.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ctisfwuo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3irzaytjo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3afybfkzf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qwiopswc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3oobpiuvd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xrtxjjzo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gdmrogtg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vowrvnfb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ezggtluc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3aroxsjpz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nbtlcnjj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mbfckqve.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3oihlsvcs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fviohzlk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ekxufkjc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vkderqjn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xssxcjck.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jfethsht.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3plopqoce.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fsxzidbh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gxmfzffr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qxaiwoyj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkrdfakb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pzyfceiz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xjqqfqeu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mmrkhhjd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kgtkalar.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3azxtaawb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eopsjfde.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3aixkdxhk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ycrmgtyd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mgoyrjca.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qsatabel.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3czcninok.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sayoeknq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gtcjmvjk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjdyohqg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bqpbcqsp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ftrlbfqw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3sczplnin.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ycoycbvl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xtnasudd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yawsllnt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bwrouetk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yjfflrdi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3azzdfgju.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wrafnech.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rbhwfjmn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ljhbltfg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xopxpojn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3euokuslg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihltrdsk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wxgoebmt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xeppoqzr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hveicbhd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3klbqylag.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcycxfsr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lsztsugj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3adwnyoyv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mpcsgqlu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zegfdbwo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3odywzcug.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gctaqfod.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3trtrlrjc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ukjghvlq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ryixmunn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3luiuzatw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3veowxwys.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3crkmwptk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ntwpehmi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jtdisxlr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ugeqoeik.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3glxhudsr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyjhrbkr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dspeknfa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3uzxslxkq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bfuxvoax.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bybxhdag.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tyburguz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lmnrdvrz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vpecqflv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3okonylov.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kdymwnmh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qjiauypx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cyynjhme.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qwqdzcyq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fmchxfjl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hurifthc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vwriklma.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vrsluvmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkwvcvzq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3abfggvzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyamhprk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fzjlqjrl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zfjruuea.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sembyeql.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wfomdofg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tndijcyq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gwytpepg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vqhdxkic.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kgjzoroq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sumxenpx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xxmlynvd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eqqxmdey.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xysmiwcm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iydqogkl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tnjvwkzu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vjmjstvl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eesoxtpz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tbxisycv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pfmepdzi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jisiaawa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vvurrxkf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fqdomjvu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vokjjpxh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hhyajxlj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxnimlfm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fsmvayjs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3olyzgnew.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zkddpmpo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3epwopxba.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hlnywawa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zkbxhapk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3negsnluw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tzpeppgf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mavblayl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3itimxpcf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3njvakzrb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zprexeke.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nysgltun.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tcmipmki.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3uavpzipm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3edagxikz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3fwkyxlrw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgtinbtb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gbykdjcv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ukperxta.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mahnnefn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ztqhyfhw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3svncbahx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bfhdqcab.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lnlwxiin.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yuqmnttp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3thtzkdjw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3baspmttz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rfqcmavu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mtwtoovn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3eyaazstr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3uiwjyboy.html


<!-- 参考信息 -->