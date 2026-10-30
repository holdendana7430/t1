代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gwspvonow.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gswyefyir.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gxtaiillr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gnrglevzu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gpoteinjq.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gekebgxvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gmvcgzppf.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gxyfaitsv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gggrodrir.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gmkktyiqk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gqlzpcuzo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gqyrcuasm.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/grfrhrlyz.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gkekqrcjq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gldzgdmcp.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gnmqqqeui.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/guahrdqqm.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gbajuvasr.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gvicqlahy.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gnyboysjg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gqewidyhd.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gpfleqkob.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gpfctnpxh.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gahthayla.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gggfeyxun.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gsrkzfwqz.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gyjgkpvfi.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/grizhygui.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gzgfeaheb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gpbkvlbng.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gguippqcs.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwdcshp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/glrjqxkpe.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gbownapao.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gycenaqxt.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/grqivtklg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gdlwakyry.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/guuaymxsg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggysxzexp.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gobfrelzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gvsnyvjvy.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwrkhyy.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/glxwoovjg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/galeconkp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gqyhxrccg.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gppplaihn.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbbzzrcsv.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gopexqfmr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/ghfvsvsid.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gffbchhqj.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/glffmidby.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gqhczhuyy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gzhecgsvo.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/ghhdobpbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gaxwbkqvf.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gsvznyslh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gjhziwkta.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gykpskjmg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gmzuvgmbm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gugfuawqa.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gvncqrkpr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/guupyddoj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gyiuyoash.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gmgzfslwo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/garzlamyl.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/grdxylafy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gwwptydmx.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gbzakeyhh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gaxhafdoi.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gpatxfwvd.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gmjygjrhh.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gdubyflkx.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gpdwjsswm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gsymuauzi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gmtbjzzdo.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gspzwdinz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gxltuemre.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gaxhmaovo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gkggruive.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gxrkjgerg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/glrlqxmki.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gfxryscfs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gauwhjyys.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/govwrdjtf.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/grtigusef.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/glmwsmkxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gfxdqierl.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gcfxjwysk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gcqhdudwm.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gxuhfnyty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gcofmrpjy.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/goflicyvd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gkwvgkval.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gqkxwssuj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/ggxhgidgi.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gngfaebfs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gphnyrtpc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gfpryhzse.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gkuuhlqxs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfsxmfqlb.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/giissoyna.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzcwlkvkc.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gaklulszm.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gkrnablcn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gmmxvzahi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gwkmmipbc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gjjwwhlud.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gptdnqxvo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gioyulczb.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gkwjipxhj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gykvtscoq.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gyyovxgap.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/glytpcmyr.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gwqydazzq.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gvzpneaad.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gzgpoppna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gjlueagnh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/grweunmed.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gxajfcylk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gmepmzwlv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gnefinkjh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gvttyjdap.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gqbaxskkk.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ggqhmbebv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gahmggjwd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gfvdoegqm.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/goffvysmv.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gvmebcter.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gmewsreue.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gulcefsqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gjsxqvsip.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gcwvlkwyp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gyekskbiu.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gmpkkvdjo.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/geeisfnjr.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gxuhxkcak.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gsrgnygxh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtuekoffh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gknuwexwq.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gohrhlpry.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/goerpqpmd.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ggegnkrgq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ggxutgpdq.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gqkffqojp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gszbmtsqg.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gjuftbrck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gfgtcuqay.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gffaqazth.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gsnnvftkw.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gezfvyrsv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gsnokbdrs.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gzqfpmfgr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gilmklpmu.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gwzgtxdmj.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gatdglbdo.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/grnjycfhx.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gwpeixepv.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gnjxxyawj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gqreirlge.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/griszwcyd.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gnnurhbvy.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gltakfoyr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gvnijjepn.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gxijjwabu.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/glihygvdd.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gedvhgjjw.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/giggepqer.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gulheuwjk.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gesgxiycw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gosmeuxge.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghrxpwerw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gcidodekq.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gquaspojk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gxjiaihwc.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gbafppppu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gicspajad.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gmzlzdaso.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gpxfilwgl.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gubaffyle.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggrkaszbb.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gygopvwgf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gcouttrlr.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/glhnkfpba.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gwvitfyel.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gluqtxtwi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gcengxedx.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/grfcijgnx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gxjelwxnk.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gqujluslg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/ginskbjzh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gottaxlev.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gplrtevcb.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gnpltrfsf.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gryftgwpf.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gfrxqlqwr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gydyibzvh.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gbwoxmeky.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/ggxwptkfj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gczuutgtz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gppnjipbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gpbyjshaa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gsjafvxjy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gshdcxdxo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gveuxddnb.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gprmtbmsb.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gzgqvhitb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gvwzcrsng.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gknuzbdgn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/griympozi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/ghkuzkaof.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/ghsfthduq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gqengkthw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gvtfcsfyv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gnokrzfkr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gcsakbrua.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gzkpuqgxx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gzzyhbbof.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gmwhepwaa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gkqxgcame.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gddoisgxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gmpjthyvx.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/grgirkkbr.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gpxzxfzcu.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/grmwniqgc.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gwzeihtvd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/giihlqfmr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gplwbaujs.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gdnfwgvvy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gudvavota.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gquoxhbgl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gkbjxzttu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbedmqpsj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/geodlaefw.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdanhyslh.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gcnxaobcb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gjwbyvbdn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gkuacssch.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gncbkaucn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/giwolnnov.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/guqukerho.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gkcnhkhxr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/ggdpixdyc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gmpakhdrb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxbmkfsio.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gbmpfnyyn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gplssyllv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/ggxxuecgu.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gkgrftzpn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gkctjllaf.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gvxiyibdj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/glihdkwdg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gltwpdxki.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gkeboxdas.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gawglxoef.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gddedcovl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gfgevapxw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gpxmvgtik.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gimmaffnz.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gnrobyefj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ghnbvooee.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/ggidknjen.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/glprdtifj.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcvdxiitt.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gwfrjbnmx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gjkcsooqc.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gwomqcaij.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gggiscxyo.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gvermxvxg.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/ganiguzqp.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/ghuebpmeh.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gcrjrychl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gbunxwdyj.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gaxzswoji.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gxlchahfm.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gghqwdzgj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gffwkdylq.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gsevjodru.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gxhpqrtkh.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gidskgzgp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gecqlzehq.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gubuljmgc.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gwolgiypr.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gfuiuyabx.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gmrmipzzy.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gctuqciyu.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/grwhtzaag.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gpfikxiyi.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gjfwxtxnl.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/guugqdylr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjavfxtw.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gpchwszdu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gkqzvlblr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbkxgtykp.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxzjlepip.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gjvpkiara.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/grkaqdmgy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/goyjtdcdq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gnkapjanv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/giywjxbgt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gfkwqfidc.sHtML


<!-- 参考信息 -->