代发 wailian999

esac
来源：http://hz.yj202588.top/gtrqjeohwk.html

[R12] for 遍历文件
来源：http://hz.cqqwz.cn/gtqenvkptl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj202588.top/gtxeshmdao.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gtwefkyjuk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtnngnmzhb.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gtnhkxdeoo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gogol.net.cn/gtasgyymss.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtcsuanjbm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangkeji.top/gtyyvvybsk.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtngfloxdf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtmpzvtqda.html

[R17] 数组定义与取值
来源：http://hz.jqgufenzy.top/gtankrhwwk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtqmtlpefw.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtgmrgnndl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtdtpjalvo.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtfflkogvn.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gtmtzldeth.html

[R20] 关联数组（字典）
来源：http://hz.yueranfly.top/gtfaargjsq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yangfankeji.com/gtuwzqrbbe.html

[R21] 字符串长度
来源：http://hz.yuanzhike.top/gtikdcrwfa.html

echo "${#s}"
来源：http://hz.316326.xyz/gtqadthsty.html

[R22] 截取子串
来源：http://hz.gaohongyu789.top/gtwtpytwej.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtmvvotsqi.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gtdcuoqbiq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pengpengdd.cyou/gtcpgbuzop.html

[R24] 大小写转换
来源：http://hz.xylfe.cn/gtnkeflbcz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtujhvkdfc.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhaomingkeji.xyz/gtifudikvu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj202588.top/gtzjjmmhym.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtowedceup.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtzxwxlskx.html

[R27] 算术展开
来源：http://hz.jqgufenzy.top/gthqffrpja.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtxhaotojh.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gtqyaafguv.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gtzbclddry.html

[R29] 定义函数
来源：http://hz.c1oappe.top/gtnnvfxnto.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtcmbiemsl.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtstlkmhje.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gtmhgvrsdw.html

[R31] 局部变量
来源：http://hz.dianchejie.cn/gtgxvesuex.html

f() { local x=1; echo "$x"; }
来源：http://hz.zycfv.cn/gttkjuonsi.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gtrltgozsg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtyzbagxxr.html

[R33] 捕获错误并提示行号
来源：http://hz.hfpthk.cn/gtmfjmungd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinyuanbaomall.cn/gtnudaccog.html

[R34] 退出时清理
来源：http://hz.gogol.net.cn/gtxxlizbfq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtdbfzpcqh.html

[R35] 后台执行并等待
来源：http://hz.yueranfly.top/gtssmrrofv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gtpaqfxhuu.html

[R36] 并发执行多个任务
来源：http://hz.jinyuanbaomall.cn/gtxfbeigsw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yangfankeji.com/gtwtmhoucc.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtjeyzobbq.html

files=$(ls -1)
来源：http://hz.jlsjyb.cn/gtneoblusd.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtstgqiowh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nwbrower.top/gtdadkkrxg.html

[R39] 重定向标准输出与错误
来源：http://hz.zhaomingkeji.xyz/gtrpbjzmuz.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtsjilmzla.html

[R40] 追加写日志
来源：http://hz.havefunace.top/gtjhmvslmt.html

echo "log" >> out.log
来源：http://hz.chenjidiqi.icu/gtgwwzpydg.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gtwlvqlsgi.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtfprxdbuu.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtgzfemyvx.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtgiunhguu.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtbzxedyyw.html

find . -name "*.log" -type f
来源：http://hz.c1oappe.top/gtanzzzwhq.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtrpmxumse.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtpavlyyfl.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtluzxjytt.html

find . -name "*.tmp" -delete
来源：http://hz.zhongyouzk.top/gtqyptbdpv.html

[R46] 递归替换文件内容
来源：http://hz.tianlin.xyz/gtysaouqxw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.c1oappe.top/gttgasvpom.html

[R47] sed 单行替换
来源：http://hz.svipenyu.cn/gthqeuznug.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gtuaxvxskg.html

[R48] awk 取指定列
来源：http://hz.chenzaomai.com/gtwytgufqe.html

awk '{print $1, $3}' a.txt
来源：http://hz.yangfankeji.com/gtvjbtdecg.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gthdwjrglx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.kuanghao11.cn/gtriixbzwa.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gteoguehoe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ehwqpu.com/gtjexfddev.html

[R51] 排序去重取前几
来源：http://hz.gotoacloud.top/gtmcryxivr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zdqjudy.top/gtdfuwqjmz.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtxgbmnxvb.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtmwghrubi.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtmqimgpsd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cucudq.cn/gtliuqhhcg.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtuxrgobuw.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtbhwnechl.html

[R55] 压缩与解压
来源：http://hz.gogol.net.cn/gtemnuosja.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtcmimcjul.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gtqzivoobv.html

scp file user@host:/path/
来源：http://hz.chenjidiqi.icu/gtwkqcoynq.html

[R57] 远程执行命令
来源：http://hz.havefunace.top/gtfohtvnmb.html

ssh user@host 'uptime'
来源：http://hz.cqqwz.cn/gtefkgyckx.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtznphqbsy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yonumen.top/gtxudgaecw.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtknucfdgz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtbmlmxehz.html

[R60] 只看 HTTP 状态码
来源：http://hz.sweek.top/gtcnvpvamr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtrjfcypkf.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gtdvwybwjq.html

df -h;  du -sh *
来源：http://hz.cdnleiting.top/gtqglmmxvc.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtpfglwkad.html

du -ah . | sort -rh | head -10
来源：http://hz.wangshuangyany.cn/gteypqtxzd.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtjlancuzr.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtnbixudsu.html

[R64] 结束进程
来源：http://hz.c1oappe.top/gthivzihfh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtmkqrnbuh.html

[R65] 查看端口占用
来源：http://hz.cdnleiting.top/gtvsrhwvvb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtgsfognio.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gtmbkqualx.html

crontab -e;  crontab -l
来源：http://hz.yj202588.top/gtxwlpzomw.html

[R67] 生成随机十六进制串
来源：http://hz.ywan-chungtsiang.top/gtbpukmybz.html

openssl rand -hex 16
来源：http://hz.redwolf501.top/gtwhredufm.html

[R68] 计算文件校验值
来源：http://hz.jlsjyb.cn/gtaypkxhva.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtzmcsivxw.html

[R69] 生成随机密码
来源：http://hz.52xcode.cn/gtzdlbeall.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigufen.top/gtqvirprje.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtvxexfdyo.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtfjdtmbho.html

[R71] 日期格式化
来源：http://hz.sufxvd.cn/gtxirhcpxy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigfzy.top/gtartkgpup.html

[R72] 等待端口就绪
来源：http://hz.aizwys.cn/gtjjnsvfnz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtmcrminyv.html

[R73] 分割大日志
来源：http://hz.shanyushiyangtech.top/gtwruegfqx.html

split -l 1000 big.log part_
来源：http://hz.ehwqpu.com/gtzevcjyaq.html

[R74] 批量重命名
来源：http://hz.hnxiangtu.top/gtzahzszzg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtmqitcaxs.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtsuaejyus.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuanzhike.top/gtxojpglrw.html

[R76] 使用临时文件
来源：http://hz.cucudq.cn/gtgslagqls.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtxusojvko.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtwvqjuqpm.html

read -rp "请输入: " ans
来源：http://hz.jiagoushi.top/gtbbthejze.html

[R78] 交互式菜单
来源：http://hz.aibaodan.cn/gtifnyduza.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigufen.top/gtuhuaxqrx.html

[R79] 解析命令行选项
来源：http://hz.yj202588.top/gtwmfcivcc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gttfxitegk.html

[R80] 查看脚本执行耗时
来源：http://hz.52xcode.cn/gtrgwzpahp.html

time ./run.sh
来源：http://hz.fengsongda.top/gtpmzakrxu.html

================================================================================
来源：http://hz.yuanzhike.top/gtwlapyjpn.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtytbajjap.html

================================================================================
来源：http://hz.nanxinkj.top/gtnkxtjvkv.html

[S01] C：Hello World
来源：http://hz.shuidangran.top/gtfycuzedh.html

#include <stdio.h>
来源：http://hz.hywenlv.cn/gthldvgcmp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtvfsjchgt.html

[S02] C：变量与格式化输出
来源：http://hz.cqqwz.cn/gtwmyiqbqf.html

int a = 10; printf("%d\n", a);
来源：http://hz.sweek.top/gtzrhqjdcg.html

[S03] C：读入整数
来源：http://hz.andypj.xyz/gtwusnizsk.html

int x; scanf("%d", &x);
来源：http://hz.jyoumei.cn/gtohzrtjxc.html

[S04] C：字符串复制
来源：http://hz.yuanzhike.top/gtgjrbhujm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtczbkldgf.html

[S05] C：字符串长度
来源：http://hz.xylfe.cn/gtkgjshalr.html

strlen(s)
来源：http://hz.nanxuanxn.top/gtzxbqpzjf.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtfctflubg.html

strcmp(a, b) == 0
来源：http://hz.andypj.xyz/gtkbsdzipc.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gttgcxgphv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gthwvecrku.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtnlbbhrih.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtjqgowwmk.html

[S09] C：结构体定义与初始化
来源：http://hz.ivvv.top/gtwcvhyofs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenjidiqi.icu/gtqgnsrcph.html

[S10] C：指针与解引用
来源：http://hz.iojbl.cn/gtawgzjzad.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtbdgojhgm.html

[S11] C：逐行读文件
来源：http://hz.cdnleiting.top/gtzkpmrrkz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtakpewtyn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtavfvacwr.html

fclose(f);
来源：http://hz.aibaodan.cn/gtykvxjyly.html

[S12] C：写文件
来源：http://hz.hysaishi.cn/gtfputkjxr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yanxiufei.cn/gthsqvbeqc.html

[S13] C：宏定义
来源：http://hz.yueranfly.top/gthpomhovy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tanke756.top/gtkhljutzg.html

[S14] C：枚举
来源：http://hz.smart0.xyz/gtrswuarkk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtrfufkhmk.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtotvfouhq.html

(double) a / b
来源：http://hz.jinghuilouyu.cn/gtoixjmblf.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gteeszupka.html

x |= (1 << 3);
来源：http://hz.jqgfzy.top/gtvawcnmzs.html

[S17] C：安全拼接字符串
来源：http://hz.zhijiandao.cn/gtaojnqqxk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangtech.top/gtmabaduao.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtfvghmboj.html

int main(int argc, char **argv)
来源：http://hz.aibaodan.cn/gtxhwolxbe.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtluhglnbp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtjkowsbdw.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtausexhhi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtgluwnocp.html

[S21] C：字符类别判断
来源：http://hz.yj20258.top/gtbfrojymh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cqqwz.cn/gtzohceudh.html

[S22] C：字符串转数字
来源：http://hz.yongpay.top/gtzwkhelbc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtseppedds.html

[S23] C：随机数
来源：http://hz.hywenlv.cn/gtifukrjhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.c1oappe.top/gthzhnsemp.html

[S24] C：获取本地时间
来源：http://hz.c1oappe.top/gtsbpzqgtr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtfltswmbq.html

[S25] C：内存拷贝
来源：http://hz.feifeiyinyue.top/gtdkcsxijv.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtmsewabdr.html

[S26] C：内存清零
来源：http://hz.sweek.top/gtopukopcc.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtajgbmovw.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtherfefzm.html

const double PI = 3.14159;
来源：http://hz.mhx1999.top/gttaytouls.html

[S28] C：静态变量
来源：http://hz.jqgfzy.top/gtljeexmup.html

static int counter = 0;
来源：http://hz.aibaodan.cn/gtciqyfrtr.html

[S29] C：变参函数
来源：http://hz.gotoacloud.top/gtblthkueq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.kuanghao11.cn/gtsscygyye.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtnsbarzxe.html

#ifndef X_H
来源：http://hz.ydzc1.top/gtcbnegimv.html

#define X_H
来源：http://hz.shuidangran.top/gtujaktcow.html

#endif
来源：http://hz.shanyushiyangkeji.top/gtuuffgjwl.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtglnxpzeb.html

#include <iostream>
来源：http://hz.andypj.xyz/gtmdxemrpe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yvedp.cn/gtnwyyqsjt.html

[S32] C++：字符串
来源：http://hz.jiagoushi.top/gthccqgild.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtvbjwjuqj.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtykxxzowf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zdqjudy.top/gtsensdmkb.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtfhrpbbsx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtuunzyhye.html

[S35] C++：map
来源：http://hz.tanke756.top/gtjofjiolh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtyqlaqxhf.html

[S36] C++：unordered_map
来源：http://hz.pengpengdd.cyou/gtkbazeqfx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtwfltfyfm.html

[S37] C++：set
来源：http://hz.dashuyun.cn/gtixevaugy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gthdlkkhhj.html

[S38] C++：排序
来源：http://hz.ydzc1.top/gteneoapkv.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gtvqsyizlk.html

[S39] C++：自定义比较器排序
来源：http://hz.dashuyun.cn/gtctjwufoj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinghuilouyu.cn/gttnvfmicn.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtsouupdmf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtkyxwahpt.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gtpzhhbhtw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.9152youxi.cn/gtupmyfavt.html

[S42] C++：继承与虚函数
来源：http://hz.hongshengwenyu.top/gtehzfygwg.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtamkeisbv.html

[S43] C++：智能指针
来源：http://hz.yonumen.top/gtinzfklii.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gteeptwfrl.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtrjrlmeea.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtojwcqcqk.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtcpygaiak.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtyaidzzvx.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtwmcuknzz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hysaishi.cn/gtabdhxbvm.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtvhpunkfe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hfpthk.cn/gtipdihvsz.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gthpqfvcij.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtfstdwjfd.html

while (std::getline(in, line)) { }
来源：http://hz.jinyuanbaomall.cn/gthlfmfgyo.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gtnzaezsrr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtpwglzvsg.html

[S50] C++：格式化数字
来源：http://hz.jianghu66.top/gtufmequej.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenzaomai.com/gtrxrkhnsw.html

[S51] C++：显式类型转换
来源：http://hz.yanxiufei.cn/gtvnlvgxys.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtomytxuwl.html

[S52] C++：const 与 noexcept
来源：http://hz.feifeiyinyue.top/gtzgkhovqc.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtimmaqrce.html

[S53] C++：移动语义
来源：http://hz.cdnleiting.top/gtftqaapxj.html

std::vector<int> w = std::move(v);
来源：http://hz.pengpengdd.cyou/gtcbotcetl.html

[S54] C++：异常处理
来源：http://hz.cqqwz.cn/gtxpmunrtx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtjxmehyzj.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtixadtjei.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yangfankeji.com/gtnafnwabv.html

[S56] C++：optional
来源：http://hz.birdmap.top/gtuuusazbc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtqmifqaob.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtmhfysxyx.html

constexpr int N = 10;
来源：http://hz.guannengcc.top/gtqpyxmjul.html

[S58] C++：命名空间
来源：http://hz.zhengqikj.top/gtdrpbdpvj.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtfytjkgdf.html

[S59] C++：静态断言
来源：http://hz.jinqigfzy.top/gtezdgiode.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenzaomai.com/gtaejijhyu.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtqxhymzmj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtnyizccxf.html

================================================================================
来源：http://hz.birdmap.top/gtfarczysj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtiynegeso.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtiutxkmus.html

[T01] Kotlin：Hello World
来源：http://hz.yuanzhike.top/gtcrewlruc.html

println("Hello")
来源：http://hz.yj202588.top/gtrhaazjvc.html

[T02] Kotlin：变量
来源：http://hz.cashguo.top/gtfvvdyysj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tanke756.top/gtokosigyu.html

[T03] Kotlin：字符串模板
来源：http://hz.jiagoushi.top/gtoaoajmuc.html

"值: $b"
来源：http://hz.ybcxt.top/gtnkgbnvll.html

[T04] Kotlin：空安全
来源：http://hz.zhongyouzk.top/gtcibbwvsv.html

val n: String? = null;  n?.length
来源：http://hz.yuxming.cn/gtfrobcecd.html

[T05] Kotlin：when 表达式
来源：http://hz.havefunace.top/gtrqcpxmgo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtwfwibsfm.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtgeanmexu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinyuanbaomall.cn/gtvmioouyc.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gtkkkkawfi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtvwttsxwv.html

[T08] Kotlin：数据类
来源：http://hz.bjfxy.top/gttbivqkyh.html

data class User(val name: String, val age: Int)
来源：http://hz.jinqigfzy.top/gtmtpmcnkb.html

[T09] Kotlin：扩展函数
来源：http://hz.gogol.net.cn/gtxgkpktmu.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gtrjxuxvtx.html

[T10] Kotlin：默认参数
来源：http://hz.xylfe.cn/gttkgudxgh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtspxshras.html

[T11] Kotlin：协程
来源：http://hz.yuxming.cn/gtvofxxovl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtrvcumuto.html

[T12] Kotlin：解构声明
来源：http://hz.zhijiandao.cn/gtqmbsvwnd.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gtysoxfpie.html

[T13] Kotlin：只读 Map
来源：http://hz.quarkkingdee.top/gtsdaordvk.html

val m = mapOf("a" to 1)
来源：http://hz.jyoumei.cn/gtjlspcvbw.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtwqbxcqmj.html

for (i in 1..10) println(i)
来源：http://hz.cashguo.top/gtezbwqeqp.html


<!-- 参考信息 -->