代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gklzgysdv.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gestvffvt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gfiobudpg.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gdnjpxtls.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gkzhsllmb.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/guahzoyqf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ggqykslip.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxbkhijvo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gvmccapze.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gsgklbezk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/grckvdqdq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gxtmlklxp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/goaffljhe.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/geerboupa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gaabvbnfl.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gbagivtpu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gwibtngwt.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gdsupkrfd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gxhsepjqd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqaiinbua.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gkybbyktd.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gnmxkqzjt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gzdhxoykt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gxdradlgt.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gfdxwnobf.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gmoqepppz.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gtwuojtmn.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gbcphlwgt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/ggekhdpdl.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/ggttihciz.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gcksqvjoo.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gevhepibp.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/geyifilor.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/glhctjndk.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gpobwhkil.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gcrlsenlg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gtteirgbj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gwryyejiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gduwrewvc.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gtqvqlxnw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/glgyvqnoj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gteskbjuc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gksthtoap.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gdwlhslwj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gwgmfahch.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gvckpvsmb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/grmmoocvw.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gafyivgqf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gdntasytq.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gyubmrqiq.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkaubqqyp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gpzaicuxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gpfqhhacj.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/giiheasaf.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/ggumdeter.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gacpmfwfg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gkmjuruio.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gkxosvzch.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gpshzqqdh.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/ghmcgtbsv.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gcolhoepk.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gwduxnpkt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gxmzqjcel.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gtlfspner.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gprjlwiie.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gunkqssvi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gdfvjksfj.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ggeuakfiq.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gzpribchy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/grvmqmwns.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gwpwiczad.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/ggegkqwki.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/guegaylkw.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/geusvifut.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/grtnctdam.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gfakgbazu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/grllmaeob.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/grgjxdarg.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gxxnxmpea.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gwawwsofy.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gqsmtaste.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gpojodezg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/goyzznilz.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gmtodkfps.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gpacwalrm.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gjjmrwkbo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gttjpmqeb.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gjiovorzl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gihyqncgq.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/ghucwnhez.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggqxfydwr.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gmfbczmcd.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gzdfasqhj.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gooqlggdm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gvmsehhfa.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gfcxswqyx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gebfzqxnu.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gecmvxjyi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gqezkvodi.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gtcyymdtk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gygyxgdyr.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gzmbxtmbo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gsqblotmk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/glrqoawqp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gvztelvhf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gpzeaqkcz.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gagctptgf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gytfbqgal.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gvfvytdah.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqjeilqfi.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmqgqpbor.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gjyavklwu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gtijeqnil.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gbgypxwdz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/glkaerlte.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gjefncghu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhljyyzd.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gdpuubrgt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gnftomhgu.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gtzeikfpg.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gjfezzjys.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ghgtmavjy.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gtomyegbz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gxosuwqhp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gyylcasau.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/grweazrpx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/glxsymceb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gvnsnecag.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gdijwoept.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gcfhxozlq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gbunmidej.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpmeaihwf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gqybicpst.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gdqkfodsf.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gqbzzdanu.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gerkdcezc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gxezzhxah.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/glftcheiy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/glcldncjm.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/griuelfae.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gwzsahphl.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gvragfgxw.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gdjvkqigf.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/ghvwcxyrh.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gzfwhzsay.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/giqaohtjw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gcbeidcby.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gxsfmhzfd.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gmdjoyfxe.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gapihiokh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/golxcheil.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gdhtjyonp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gcjddxlmr.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gufjvcsdj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gyhzdokrd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gdjanoskz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gafbyimqe.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gtsyzptrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/ggeinqfub.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gsrylixlp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gavipswco.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gwwvarnje.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gjzkzfles.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gsuabhglk.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gzcxxdikj.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gmiihdirm.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqfspvfms.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gqlmzlhvi.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gddlkyqjs.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gyxsnnphx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/grhgfennv.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gyvfjdmaw.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gnimtvxlb.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gzbforgnq.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gpnbdmzkl.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gznseuone.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gwtzdbozt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gfajqlphu.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtcytddzu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gfqujrjwm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gsiwgsabg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gpzntvexf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/grqxjcidh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gypawnagc.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gbastxskq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmhvnafnp.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gexvhbzpc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gaaspbmdb.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gnmqzngud.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gyycxqrjk.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gcrnkexqp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvvwklgmd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gmqtbpzow.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gpdcdnjyc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqzrxhojq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gvignhglo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/goiupucfh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gbzofzjqv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gmxwsdwkg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/geczlebgx.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/ggkjbkumz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gvacytivs.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gtbstuoqs.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gzogpcrkp.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ggbeifvss.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/grmnjpfgz.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gwoyvnmpb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkwtnwaiz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gdsuklcvy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gczhnqtod.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqlenpisd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/grclivbcv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gwcpvvtym.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gyajkopre.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gqcvzqtqn.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gcpvlrlye.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gudauzxfq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gdfqvnrom.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gzhudmams.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/glqodpgfe.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/ghgsbmyyd.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gomjlmaec.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gfvtwtruv.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gripejieg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/ghqyvwnom.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gvhyotpfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/glcmeghbc.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gimfriklc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gbvskzotn.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/grwalapde.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gahfkidbz.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gcxjnmyjw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/garrinpkm.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gmaquxogz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gujhoarfq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gfbutmgwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gtwumjamb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvbbfvuje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/giqrhtrmc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grpvrldzb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/glqtznfcr.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggbfnlqit.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gczaetzxc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/giioecgel.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gqoxpnomi.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gkjscwrom.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gxguymmtr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gwigvnxbt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gayxonokl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gzlxlxils.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gkruobfns.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gmsqluoub.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gswmzgnzl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gthuaryqk.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gpzwumknf.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gcjbjbnmz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/giomxdgas.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gsnnsubwm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gbbrjdpwg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gsoombojg.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gsqowwaor.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gmgazztbu.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gbbkcagjn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpewhdtmb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gxcdjlgwc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gpuounylo.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gedylhnil.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gjxwxrtcx.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gtlrcfkmb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gezwhewex.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gcanqnkbm.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gmiqevsfy.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gkvscdhke.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/giexhvtgr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gvfkigwem.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gnmqkdpqd.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gkthmwltm.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/glcrzkncd.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gvbzkaetz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gfopwnmum.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/ghgrozbuj.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gkbetgpxc.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/goovtymlx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gwrpbqrnq.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gbzltqhod.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gawummvmx.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gootjavxw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gbotpfnno.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gwfdizwny.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/grwpigyql.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gpjupsqcq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gouwxbtrb.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/grxrsatmp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/ggiwleqix.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gtoftgwfc.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gojjltprp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/grmtqtakr.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gbqqrdrud.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gwefxxmdr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gfmocomts.sHtML


<!-- 参考信息 -->