代发 wailian999

case "$1" in
来源：http://hz.tian-w.cn/gtthbreabv.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtfoiwcjif.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gtmorxuxtn.html

*)     echo "未知命令" ;;
来源：http://hz.cashguo.top/gtyossbgph.html

esac
来源：http://hz.cheryme.top/gtjgobhioa.html

[R12] for 遍历文件
来源：http://hz.vqdsnc.cn/gtrlfbuqwj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zycfv.cn/gtxvzftgbq.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtfaxjvwde.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sysykeji.top/gtpmvrkyth.html

[R14] C 风格 for
来源：http://hz.yangfankeji.com/gtrhvcalwy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtmohduosq.html

[R15] while 逐行读文件
来源：http://hz.fzhhl.top/gtijjwmhat.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yvedp.cn/gtphjoyepa.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtgwwfjydb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aizwys.cn/gtujzyoplg.html

[R17] 数组定义与取值
来源：http://hz.hysaishi.cn/gtjxtcvvup.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.52xcode.cn/gtujfqmgis.html

[R18] 遍历数组
来源：http://hz.yj20258.top/gtexcsiqgq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gtbyreeeyp.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtcqfzfrmk.html

echo "${#arr[@]}"
来源：http://hz.aibaodan.cn/gtpplkxvuk.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtvzzwhbqb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cucudq.cn/gtaagvtzne.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtiwvbshhc.html

echo "${#s}"
来源：http://hz.dashuyun.cn/gtuweqfeqs.html

[R22] 截取子串
来源：http://hz.yueranfly.top/gtizemijqi.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtftrarbpd.html

[R23] 字符串替换
来源：http://hz.ivvv.top/gtirgxtriz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.snrcjt.cn/gtwsjyyhpo.html

[R24] 大小写转换
来源：http://hz.kuanghao11.cn/gtxfrprzyb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.mhx1999.top/gtblntjpug.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtaxioirim.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jlsjyb.cn/gttitwmvpn.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gtwchkcowf.html

now=$(date +%F); echo "$now"
来源：http://hz.jyoumei.cn/gtlbarygsw.html

[R27] 算术展开
来源：http://hz.jiagoushi.top/gtcmwrxawe.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtwvmacwqb.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtwkatkaqa.html

echo "scale=2; 10/3" | bc
来源：http://hz.nwbrower.top/gttjzilggw.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gtrqqaxeoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtglwhusuc.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtgdhzgnnt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.smart0.xyz/gthatvrcho.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gtzbtqpiox.html

f() { local x=1; echo "$x"; }
来源：http://hz.haohaochexian.top/gtoninemqe.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtswiorydq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtroofqlfq.html

[R33] 捕获错误并提示行号
来源：http://hz.quarkkingdee.top/gtfjatjkza.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gogol.net.cn/gtjoqrtimx.html

[R34] 退出时清理
来源：http://hz.daxiang520.top/gtisoabpxi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gttnvbhjlw.html

[R35] 后台执行并等待
来源：http://hz.zhixingplan.top/gtgnoldqrw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgfzy.top/gtjzhnefvu.html

[R36] 并发执行多个任务
来源：http://hz.hnqzz.top/gtxxcjsmix.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gtdxuqvfgd.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtlppwbxcu.html

files=$(ls -1)
来源：http://hz.bjfxy.top/gtyzpkwedm.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtbqgmnzql.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guannengcc.top/gtrdslnrfg.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtbbrytydy.html

cmd > out.log 2>&1
来源：http://hz.vqdsnc.cn/gtbfthmlus.html

[R40] 追加写日志
来源：http://hz.cqqwz.cn/gtzotbehhw.html

echo "log" >> out.log
来源：http://hz.yueranfly.top/gtrxuvramm.html

[R41] 丢弃输出
来源：http://hz.gogol.net.cn/gtjbukzujj.html

cmd >/dev/null 2>&1
来源：http://hz.daxiang520.top/gtghqgbwkt.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtfcitutgd.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtpydipsbn.html

[R43] 按名字查找文件
来源：http://hz.fengsongda.top/gtkzvdkoib.html

find . -name "*.log" -type f
来源：http://hz.aizwys.cn/gtugcxigjv.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtxpvvootq.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtmzqeapsg.html

[R45] 批量删除
来源：http://hz.vqdsnc.cn/gtipofgayb.html

find . -name "*.tmp" -delete
来源：http://hz.yanxiufei.cn/gtmeikagwq.html

[R46] 递归替换文件内容
来源：http://hz.tianlin.xyz/gthufyhyxq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj202588.top/gtotryiwnn.html

[R47] sed 单行替换
来源：http://hz.yj20258888.top/gthbjdbnom.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.quarkkingdee.top/gtfhxkyeqg.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtyxlqsylz.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtpabgtkgp.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtziwnbgfg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangkeji.top/gtsbpkzutj.html

[R50] awk 求和
来源：http://hz.yuxming.cn/gtsrmjxkxv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydjk.org.cn/gtjucedhfd.html

[R51] 排序去重取前几
来源：http://hz.dashuyun.cn/gtalubghzc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hammf.cn/gtllxxlqci.html

[R52] 统计行数
来源：http://hz.zhiwuduotai.top/gtelvpywlm.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtevernati.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtebqfefmp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gtuhejkokl.html

[R54] 比较两个文件
来源：http://hz.316326.xyz/gtuikskfgs.html

diff a.txt b.txt
来源：http://hz.zhijiandao.cn/gtdxlikwae.html

[R55] 压缩与解压
来源：http://hz.jqgufenzy.top/gtfdyyatei.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guowangkeji.top/gtedfdetdz.html

[R56] 远程拷贝
来源：http://hz.sysykeji.top/gtgukdgizv.html

scp file user@host:/path/
来源：http://hz.chenjidiqi.icu/gtzdgxhpeo.html

[R57] 远程执行命令
来源：http://hz.jqgufenzy.top/gtaxzeanvo.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtqwzynpxg.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtrxuotdso.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sufxvd.cn/gtyxusdjev.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangtech.top/gtdvuqgdio.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtkihwojcy.html

[R60] 只看 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtxeoojlzr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtbenzdrip.html

[R61] 磁盘占用
来源：http://hz.hnqzz.top/gtdmdpvtyh.html

df -h;  du -sh *
来源：http://hz.iojbl.cn/gtprubnvkg.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gttshlqjqb.html

du -ah . | sort -rh | head -10
来源：http://hz.yuanzhike.top/gtoitnxmxb.html

[R63] 内存与进程
来源：http://hz.ppjwa.cn/gtdrtfyhwq.html

free -h;  ps aux | grep nginx
来源：http://hz.ybcxt.top/gtdctrfxkk.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtbrvlfmvu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtsinbhckf.html

[R65] 查看端口占用
来源：http://hz.daria6918.cn/gtpspakqzp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtfmgkwvsu.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtgczjklzf.html

crontab -e;  crontab -l
来源：http://hz.yuxming.cn/gtpwqghdht.html

[R67] 生成随机十六进制串
来源：http://hz.jiagoushi.top/gtpiyitxqo.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gtrxvnypab.html

[R68] 计算文件校验值
来源：http://hz.zdqjudy.top/gtimacfqqi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtxexpneey.html

[R69] 生成随机密码
来源：http://hz.zycfv.cn/gtvnkiedvb.html

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gttzacibtu.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtrievrtao.html

date +%s;  date -d @1700000000
来源：http://hz.smart0.xyz/gtgnsdqued.html

[R71] 日期格式化
来源：http://hz.xziqi.cn/gttmjncaqo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangtech.top/gtqmtpifle.html

[R72] 等待端口就绪
来源：http://hz.zycfv.cn/gtarggycin.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj202588.top/gteaygvzhd.html

[R73] 分割大日志
来源：http://hz.zhiwuduotai.top/gtzxltmmbq.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtnqdhwkra.html

[R74] 批量重命名
来源：http://hz.zhijiandao.cn/gtvdvhbanu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dianchejie.cn/gthhgojayh.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtuxabpjhd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.fzhhl.top/gtcotsvnaz.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtwunzaaux.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtgeghaapi.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gtbteqwabi.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gtbeeamlje.html

[R78] 交互式菜单
来源：http://hz.hnxiangtu.top/gtkoflfoig.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtnrosfmxr.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtshbwxvsk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xingfuxueyuan.xyz/gtmqnfcdzo.html

[R80] 查看脚本执行耗时
来源：http://hz.birdmap.top/gtoevcsguf.html

time ./run.sh
来源：http://hz.cucudq.cn/gtqnsuzqbg.html

================================================================================
来源：http://hz.cucudq.cn/gtrtpgmndd.html

S. C / C++ 专题
来源：http://hz.hfpthk.cn/gtdihbzhhy.html

================================================================================
来源：http://hz.jianghu66.top/gtmzsymwfv.html

[S01] C：Hello World
来源：http://hz.daxiang520.top/gtvnkklafm.html

#include <stdio.h>
来源：http://hz.tanke756.top/gtensojden.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gtmiboygwn.html

[S02] C：变量与格式化输出
来源：http://hz.hammf.cn/gtvuzvywcm.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtgwvljwsi.html

[S03] C：读入整数
来源：http://hz.hfpthk.cn/gtamegfcnu.html

int x; scanf("%d", &x);
来源：http://hz.feifeiyinyue.top/gtkftfqxhd.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtfhzzkwcz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gthcxvkhgo.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtpsgpbnoa.html

strlen(s)
来源：http://hz.yueranfly.top/gtwhimxgta.html

[S06] C：字符串比较
来源：http://hz.meibo888.top/gtvksggwvt.html

strcmp(a, b) == 0
来源：http://hz.feifeiyinyue.top/gtyruhfdgd.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtpzousspz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fengsongda.top/gttfaokjkf.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtyumyxbym.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.bjfxy.top/gtsflrjnkv.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtjmqjvhqz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtbixbkckr.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtqrctknwf.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtlzlbghyf.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtzdwpxfde.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtteduvguy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pengpengdd.cyou/gtoeesnfyf.html

fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtismfbhvb.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtpbnmjeup.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aizwys.cn/gtjhpmygdr.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtyznrxuxm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtzuzpvyti.html

[S14] C：枚举
来源：http://hz.316326.xyz/gtozttkwjm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cdnleiting.top/gtrtctoqdo.html

[S15] C：类型转换
来源：http://hz.dashuyun.cn/gtogvgmkva.html

(double) a / b
来源：http://hz.jlsjyb.cn/gtmciupelk.html

[S16] C：位操作置位
来源：http://hz.jinqigfzy.top/gtzvmtuhae.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtcfrzwtxb.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gttgxdqcey.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtppeligwk.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gttxynqlph.html

int main(int argc, char **argv)
来源：http://hz.redwolf501.top/gtcvyahaqh.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtutgywalc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtfyrdynfm.html

[S20] C：二分查找
来源：http://hz.jianghu66.top/gtibnkgjma.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtybpddwvf.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gtebgjaqwc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.feifeiyinyue.top/gtjkclrfsz.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gthrouwtxg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtovkisqnp.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtrsmmqxem.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gttxdarosz.html

[S24] C：获取本地时间
来源：http://hz.vqdsnc.cn/gthtaynrlr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shuidangran.top/gtacxpclls.html

[S25] C：内存拷贝
来源：http://hz.yueranfly.top/gtcseqmaqf.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gthdtycpvn.html

[S26] C：内存清零
来源：http://hz.xuetiantiany.cn/gtebmbyryk.html

memset(a, 0, sizeof a);
来源：http://hz.tian-w.cn/gtxxirfmwv.html

[S27] C：定义常量
来源：http://hz.ydzc1.top/gtfqlyijks.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtvozoaayh.html

[S28] C：静态变量
来源：http://hz.ywan-chungtsiang.top/gteritpyhx.html

static int counter = 0;
来源：http://hz.ehwqpu.com/gtrbczxrtd.html

[S29] C：变参函数
来源：http://hz.nwbrower.top/gtoqoxgvxr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtyjzdhmed.html

[S30] C：头文件保护
来源：http://hz.ivvv.top/gtkjebzfqt.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtamrblkcv.html

#define X_H
来源：http://hz.dashuyun.cn/gtsxjxpirh.html

#endif
来源：http://hz.quarkkingdee.top/gtrkrnqgfu.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtmfwxcayg.html

#include <iostream>
来源：http://hz.dashuyun.cn/gtyogrkmnl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtnlqorfud.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gttaaaccfq.html

std::string s = "hi";  s += "!";
来源：http://hz.zdqjudy.top/gtcgynysvq.html

[S33] C++：vector 增删
来源：http://hz.snrcjt.cn/gtkiktgbqs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhoulong.xyz/gtrzzuttno.html

[S34] C++：遍历 vector
来源：http://hz.fzhhl.top/gtcklzrypu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtkxbvrutm.html

[S35] C++：map
来源：http://hz.gaohongyu789.top/gtubzsztfu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtejdwfbjh.html

[S36] C++：unordered_map
来源：http://hz.yanxiufei.cn/gtylvyfghx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtkemeihqh.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtnvzyvjai.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtyamwktfd.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtvrqkbrpu.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258888.top/gtzamdoouf.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtyhspmxqz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dianchejie.cn/gtoglnzgww.html

[S40] C++：查找元素
来源：http://hz.yonumen.top/gtsaircnhh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gtcgqioykx.html

[S41] C++：类与构造函数
来源：http://hz.xingfuxueyuan.xyz/gtgwaywyox.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangshuangyany.cn/gtwjniwkgo.html

[S42] C++：继承与虚函数
来源：http://hz.0kj1m.cn/gtnonjlyrn.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gtyyuszyku.html

[S43] C++：智能指针
来源：http://hz.fzhhl.top/gtjdjvmphg.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenzaomai.com/gtbcdjuoti.html

[S44] C++：引用传参
来源：http://hz.yuxming.cn/gtunrbjkcu.html

void inc(int &x) { ++x; }
来源：http://hz.jinghuilouyu.cn/gtxewcsayo.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtvthcmubc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fzhhl.top/gtcqnpdptr.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtctnemhuw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gttweqozdc.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtellciuow.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hysaishi.cn/gtjstwlpux.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtkydqwlmx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtopmiufkc.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtkzkucsun.html

[S49] C++：写文件
来源：http://hz.zhongyouzk.top/gtswbkaaee.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xylfe.cn/gthbgydinm.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtgmmttcxb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gtxiseideh.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtapgewong.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtmbazcanv.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gtmukrrcwo.html

int size() const noexcept { return n_; }
来源：http://hz.zdqjudy.top/gteiwtemuv.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gtfbmlqjnm.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gtzktezdmq.html

[S54] C++：异常处理
来源：http://hz.snrcjt.cn/gtkitpwdjc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jianghu66.top/gtscdovbvx.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtdzlomtsc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hysaishi.cn/gtewnfnotq.html

[S56] C++：optional
来源：http://hz.hfpthk.cn/gtyafpoyba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gttffhaols.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtknqbyorq.html

constexpr int N = 10;
来源：http://hz.sxryk.cn/gtgcozdcnh.html

[S58] C++：命名空间
来源：http://hz.fzhhl.top/gtqzzbkcoa.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gtlspbshtf.html

[S59] C++：静态断言
来源：http://hz.c1oappe.top/gtqtnsqxjo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuxming.cn/gtwedncnow.html

[S60] C++：遍历并删除元素
来源：http://hz.chenjidiqi.icu/gtqfplxpaj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenzaomai.com/gtwzdwcdhw.html

================================================================================
来源：http://hz.cheryme.top/gtohmwrabw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtvyeelabs.html

================================================================================
来源：http://hz.316326.xyz/gtdzzxesxs.html

[T01] Kotlin：Hello World
来源：http://hz.chenlongwang.top/gtdqvspvyc.html

println("Hello")
来源：http://hz.zhixingplan.top/gtprqtwuti.html

[T02] Kotlin：变量
来源：http://hz.chenjidiqi.icu/gtearvrhsc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hfpthk.cn/gtghthqmiv.html

[T03] Kotlin：字符串模板
来源：http://hz.kuanghao11.cn/gtdpqqgthx.html

"值: $b"
来源：http://hz.yj202588.top/gthwozzodg.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtlovniwrb.html

val n: String? = null;  n?.length
来源：http://hz.yj20258.top/gtczeomvfp.html

[T05] Kotlin：when 表达式
来源：http://hz.yvedp.cn/gttyhxsmdv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daria6918.cn/gtsjsczffb.html

[T06] Kotlin：集合映射
来源：http://hz.zhiwuduotai.top/gtvhcyywli.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ybcxt.top/gtjbckadzh.html

[T07] Kotlin：集合过滤
来源：http://hz.pengpengdd.cyou/gtkvspbsrn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtraefruus.html

[T08] Kotlin：数据类
来源：http://hz.gotoacloud.top/gtgczjftcv.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtuyenckyx.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtkrwwlamz.html

fun String.exclaim() = this + "!"
来源：http://hz.pengpengdd.cyou/gtpeuuvokx.html

[T10] Kotlin：默认参数
来源：http://hz.birdmap.top/gtirmlhmgv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtvbeqviag.html

[T11] Kotlin：协程
来源：http://hz.chenjidiqi.icu/gtgoxumrof.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.smart0.xyz/gtozduxcql.html

[T12] Kotlin：解构声明
来源：http://hz.shzxlz.cn/gtfovthzie.html

val (a, b) = Pair(1, 2)
来源：http://hz.ehwqpu.com/gtrctwwrlj.html


<!-- 参考信息 -->