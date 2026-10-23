代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vrnibfkc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vfvojheq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3izybkjoy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdvzybkl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhzkgxob.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3eziaxqlx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iiezmowk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sfxdttup.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kdywcpab.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3igifzzxx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vxmyxgut.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lppsmwvg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zagcqezw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3udygfgeg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3uktcstjc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xpyysxaz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3siujahvx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ikfjbtsu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wcpuceek.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3blrvxnvo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ueavsuca.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nlpscdun.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3cntgrnjj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mqbcziji.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cmcumttj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rmiosrlp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3idmjftku.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3anfexmlw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tfdxiyzo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tibsmpgo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3liahitbt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vklpvznv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3tjnohnlm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iaqapvmw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3eofbwyok.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ivulvovo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3flaakjmx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mrlmglob.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3alpayfxl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yrdchyrc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hzlmzcvm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3axoglldh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3byukglxb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3itggmvrs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3eoszlbxo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rclpznbh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kdxwkgug.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3afwbqavd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vojfykfy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwfuvgxc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jhgygxji.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zhfqakvu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uywlslrj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pdxnlkke.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cqoksrzp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bvrnbvqb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3tevwinap.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mqpuafrm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nnkxttmu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jlfjfcfa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xrystegl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3okpsiqza.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pjmddeic.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nedaafsz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bcqvrlak.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3umhyoexd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wqvxhbai.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3brvuhlim.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jvflmzjk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gyimdcsu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rkuftyhd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hihljshs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3avxznbnl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bspxvfwm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3lnjhbwho.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vgnjhvxf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xsgmhoic.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3aihcrjnz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3grnylwlk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iqsiynzx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qvzrtfbr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nyipaoam.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dqbgbyuh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lnwpjczc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nwpfhvgp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3laulrwwu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hkwmhzoo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nlfcoatb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3inrmeztf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3quplvthe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rsjwnujl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kkqbzphx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gokspqin.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zjyxuiee.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mxptuuvh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3djglqejm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3oxmqjiog.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yvqkozxt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jjupxfpr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tyingzvf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3slkhkotm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3itwhrgac.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kauplryu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lplzgmiu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iioecdac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrilumbz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rrgyvfel.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vszzufna.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxzymbrh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3alhkenin.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zwfodvlm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kogcxxyv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nwzxkebj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3gqbrusaw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lnbnqjwy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hrrtgvxr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cfxhdpng.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vfmpighy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gqffcfcp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xzklfico.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3negpxaqb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rwfnbydi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rfezeghd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kcrvliow.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3stvkfmhc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vbqdsjdu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3frriptsd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbktkooh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3usxjtikg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tzxuhubp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dartbrun.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ceinjhxs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kxbglycz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yxbaiuuo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fdorhcjn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ojwbswea.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wicqtjdt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aapksopx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wabglewi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fxivnfoe.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rwdxyhex.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uysjdaiu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nqwigowc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gzolerpp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lduwfxff.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3itogpieu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sayeiyrx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rdwrkcel.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kjscqqmy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qqbtmsst.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hwfbrztb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lovstcet.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jpohiapv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ygcsgzfr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3smlwxnvc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xeniqzls.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zpqlucme.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vikisxqi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3edkqhuoc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yalnxhax.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3duxdfgmz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lmqkhibc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vrmerdmo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ivjerppw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qlartxsh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wsmqxvkq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3luzhjyxn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pijpjgmj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mkhckhqj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bshibhfe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3egwpsqiw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3louckpgl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ftibaefk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3orjnjjyb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wlqzeykl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lgemsirz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3alzjggqd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bmhyseiq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tirecatw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3psyehuuy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vmrejmgs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wczzaepd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ojprarul.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rbpozmkh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gbxrdfrw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qvnrsfih.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cfddmoeu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ykbwhxcu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iwqqxipt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qjfpuzux.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xhetgoti.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xmnzlkve.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bicfwzlg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rfjzztst.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3usznlrrw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tcugrmyx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ztcrdzea.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ukgprjyq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bnqnprin.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3orpntqbh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qjevhwlf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oiidgfhi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3iojchiji.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qiwzfoar.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3azrknlce.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tiyefanf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rkrwslul.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3atdnemcv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wganylyi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3uecvbija.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vrjyjawv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3uwwlushp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gfljetjp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pxnzdgzh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3likljxyk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jyaqvgvn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3eljcrtrh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vwdgbgda.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mietgqrf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3miulfoyo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ryrrvqiw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uxhnmpki.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3latwxbce.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ndyyumfb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zcuwlpij.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3iianqxbp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vttqkjui.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qyfgxeta.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fdvgrtmd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ilrorfnv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wtiptiaa.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3soittnqr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lbnootrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxxadrcw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3czecojrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbpsymmu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ywrmeesu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hnffpoqv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mjeifuvh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zpnpsdhq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3lfroeydv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hibouvxg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fsnqxhxp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3aembmejm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rsuujfex.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bylqeuuy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sogifcvf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mtqefsbq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jkixunah.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3aqfcqjwf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3flcsthom.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kwoqphxz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxncglui.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3adbacadu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3czjcqjsw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xfjpurgo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3readhvyy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ebfpsdfn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jtnvmtms.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qnilvrfs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xrosprya.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqdeyyp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rjfifbtc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hqrmperk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gugxpapp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3trvdnphv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rzlrcczh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qugeacgd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3upjlxugm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gspoxdcz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mpthrohx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xbtsszvh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fyczhfff.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3koynexix.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ekstvasi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vxwqpsvn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bzsbqjtt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3iwpmvwtd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nrwtcsas.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rhxstcxa.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3aiixlwom.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lqhiupfz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jusqxjnm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvsffvp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fqdxlebs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jicfroto.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ynzdtzoi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3avrswbbh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3lndzvfcm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gkaagibk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ksgwgkcf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3oltiosgq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cqzqtkiy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fzuwvwqr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mkfeqybj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jnwuvlkc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gzogccyw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kkkwroas.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lrwlcwug.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3meyiexde.html


<!-- 参考信息 -->