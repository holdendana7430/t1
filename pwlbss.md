代发 wailian999

case "$1" in
来源：http://hz.316326.xyz/gttmrvxtbb.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gteiwmpuyl.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gtrmeasbls.html

*)     echo "未知命令" ;;
来源：http://hz.c1oappe.top/gtrsomjuir.html

esac
来源：http://hz.hnxiangtu.top/gtfoqxbtww.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtqwtivsdb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtfiacprss.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtsxmsyhnl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gtodabifxv.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtbzzgwflz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gtczysremq.html

[R15] while 逐行读文件
来源：http://hz.jinqigfzy.top/gtnubpcgwh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtzhtbbfjg.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtusftohrk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtciyxlayr.html

[R17] 数组定义与取值
来源：http://hz.mhx1999.top/gtkprpiyla.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tian-w.cn/gtirfcriqv.html

[R18] 遍历数组
来源：http://hz.ydzc1.top/gtajfgufaz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zdqjudy.top/gtpvaqbpdf.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtrdbtpmse.html

echo "${#arr[@]}"
来源：http://hz.aibaodan.cn/gttnbhwjsm.html

[R20] 关联数组（字典）
来源：http://hz.zdqjudy.top/gtabcdjoxy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenlongwang.top/gthiwhslmh.html

[R21] 字符串长度
来源：http://hz.zycfv.cn/gtbwcutxep.html

echo "${#s}"
来源：http://hz.hongshengwenyu.top/gttmvjmvdh.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gthozxkkgk.html

echo "${s:0:5}"
来源：http://hz.snrcjt.cn/gtowprivsw.html

[R23] 字符串替换
来源：http://hz.pengpengdd.cyou/gtslgxbhty.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hammf.cn/gtzfreihoc.html

[R24] 大小写转换
来源：http://hz.cheryme.top/gtysbmmbcc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.snrcjt.cn/gtgdghkbaf.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gthlnetwyc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.quarkkingdee.top/gtdosiikez.html

[R26] 命令替换
来源：http://hz.aibaodan.cn/gtroebawaj.html

now=$(date +%F); echo "$now"
来源：http://hz.sxryk.cn/gtopfklwuq.html

[R27] 算术展开
来源：http://hz.gogol.net.cn/gtnhmwormq.html

echo $((1 + 2 * 3))
来源：http://hz.pengpengdd.cyou/gtkyyrwbzd.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtkunssayz.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigfzy.top/gtgxlrvypy.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtugcacgcm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtilehwyir.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtiasdpqvr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhijiandao.cn/gtpnlukjws.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtwvheixsy.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gtbagfctmf.html

[R32] 参数个数校验
来源：http://hz.aizwys.cn/gtrzmmlcdp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gteoxcxmnn.html

[R33] 捕获错误并提示行号
来源：http://hz.andypj.xyz/gthexicsye.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gzhubu.top/gtzxlgfazp.html

[R34] 退出时清理
来源：http://hz.feifeiyinyue.top/gtqmzntcae.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guannengcc.top/gtzjsrmwob.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtncrqxqke.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtfgwljgyz.html

[R36] 并发执行多个任务
来源：http://hz.ivvv.top/gtqfjgafey.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangkeji.top/gtohoczfxl.html

[R37] 把输出赋给变量
来源：http://hz.9152youxi.cn/gttpihcgvc.html

files=$(ls -1)
来源：http://hz.guannengcc.top/gtjqrnakwg.html

[R38] 管道串联
来源：http://hz.ywan-chungtsiang.top/gtflajonup.html

cat a.txt | grep -i error | wc -l
来源：http://hz.316326.xyz/gtjxaldmoq.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtbrtelovh.html

cmd > out.log 2>&1
来源：http://hz.pengpengdd.cyou/gthihtdacn.html

[R40] 追加写日志
来源：http://hz.nanxinkj.top/gtuepfvxtz.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtmvzngvxg.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtbuulukjh.html

cmd >/dev/null 2>&1
来源：http://hz.yueranfly.top/gthjniiptp.html

[R42] 输入重定向
来源：http://hz.hongshengwenyu.top/gtlhrxsepf.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtryanzybf.html

[R43] 按名字查找文件
来源：http://hz.dianchejie.cn/gtaqaihduk.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtivkqjmex.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtmbvdqdvy.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtzpqbxcnc.html

[R45] 批量删除
来源：http://hz.redwolf501.top/gtrvrzbmvt.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtvejgyipw.html

[R46] 递归替换文件内容
来源：http://hz.xuetiantiany.cn/gtjnprqcai.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.vqdsnc.cn/gtfjywylhg.html

[R47] sed 单行替换
来源：http://hz.zhengqikj.top/gtwqhkyfdh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pengpengdd.cyou/gteletyemu.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtzzyfgasp.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtoviwlyob.html

[R49] awk 带条件
来源：http://hz.jianghu66.top/gtirpkdobm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yangfankeji.com/gtbkxigshl.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gteesbazls.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtqrivkwrl.html

[R51] 排序去重取前几
来源：http://hz.nwbrower.top/gtwjrphmrv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtebomlvwc.html

[R52] 统计行数
来源：http://hz.jyoumei.cn/gtvmpqengj.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtadwtyrgj.html

[R53] 查看文件头与实时尾
来源：http://hz.cdnleiting.top/gtgxvmtxly.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtmfukcfqi.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtftcswaiy.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtqsrnhljv.html

[R55] 压缩与解压
来源：http://hz.quarkkingdee.top/gtewktrdks.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gthsktmcap.html

[R56] 远程拷贝
来源：http://hz.jinghuilouyu.cn/gtjowqnltt.html

scp file user@host:/path/
来源：http://hz.birdmap.top/gtuaodjfvc.html

[R57] 远程执行命令
来源：http://hz.smart0.xyz/gtprchihkf.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtqiwxlfex.html

[R58] 下载文件
来源：http://hz.jlsjyb.cn/gtkypzcjrb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gotoacloud.top/gttljbsmlw.html

[R59] 发 POST JSON
来源：http://hz.pengpengdd.cyou/gtbnenhqnw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtlamirkci.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtyhqkkpbg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtzwzszhfs.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gtueaanxcs.html

df -h;  du -sh *
来源：http://hz.xuetiantiany.cn/gtlgfsqbfa.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtzztpyjcr.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtrvwqndql.html

[R63] 内存与进程
来源：http://hz.sysykeji.top/gttgmvzhqy.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gtlxvuvslm.html

[R64] 结束进程
来源：http://hz.ywan-chungtsiang.top/gtcwhjitum.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xingfuxueyuan.xyz/gtgluehnmf.html

[R65] 查看端口占用
来源：http://hz.xingfuxueyuan.xyz/gtuqgxhxxa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtrsuqcngv.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtygecrlwr.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtuqffaefo.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtecuuhjtb.html

openssl rand -hex 16
来源：http://hz.kuanghao11.cn/gtwmigntzy.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtukzbyrxn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jiagoushi.top/gthcdribvn.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gtsgekppkv.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtuottgter.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gthyrrldgh.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtggxnrehm.html

[R71] 日期格式化
来源：http://hz.jyoumei.cn/gtlqebjkde.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.svipenyu.cn/gtamtwtkij.html

[R72] 等待端口就绪
来源：http://hz.sufxvd.cn/gtezepesdz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtchghuoos.html

[R73] 分割大日志
来源：http://hz.ydzc1.top/gtljgauxbc.html

split -l 1000 big.log part_
来源：http://hz.hnqzz.top/gtzznhtkdp.html

[R74] 批量重命名
来源：http://hz.zhijiandao.cn/gtnverxmko.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daria6918.cn/gtojozddzy.html

[R75] 导出环境变量
来源：http://hz.jqgufenzy.top/gtfonzdltb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgfzy.top/gtpiewgpfq.html

[R76] 使用临时文件
来源：http://hz.quarkkingdee.top/gtoaroccwr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtxgqskgpu.html

[R77] 读取用户输入
来源：http://hz.chenjidiqi.icu/gtshkuqiip.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangkeji.top/gtuffkpxyc.html

[R78] 交互式菜单
来源：http://hz.jyoumei.cn/gttqpjczqw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aibaodan.cn/gtovuimzsi.html

[R79] 解析命令行选项
来源：http://hz.kuanghao11.cn/gttznhurlj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhengqikj.top/gtoydmbugu.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gtpjsalbqi.html

time ./run.sh
来源：http://hz.316326.xyz/gtpcnqjeau.html

================================================================================
来源：http://hz.316326.xyz/gtcmhjsvcr.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gtbdfrrmfd.html

================================================================================
来源：http://hz.yj202588.top/gtxnglstpg.html

[S01] C：Hello World
来源：http://hz.zdqjudy.top/gtjwywcazw.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtjpbgrciu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gtzkntlevc.html

[S02] C：变量与格式化输出
来源：http://hz.dashuyun.cn/gttdcooubn.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigufen.top/gtjhzvqhdr.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtvtkyrkbz.html

int x; scanf("%d", &x);
来源：http://hz.zhijiandao.cn/gtclsbuzeo.html

[S04] C：字符串复制
来源：http://hz.yuxming.cn/gtznmoeayw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnqzz.top/gtuxmtpvuo.html

[S05] C：字符串长度
来源：http://hz.sweek.top/gtgxcdpcqb.html

strlen(s)
来源：http://hz.haohaochexian.top/gtsbujrpxh.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtjzxqvkta.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtqnyhakzi.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gtdacdbiah.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtgvnpwwnj.html

[S08] C：动态内存分配与释放
来源：http://hz.hammf.cn/gtttqtbndu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtilgssgcb.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtliigpjos.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.smart0.xyz/gtdlamvpnd.html

[S10] C：指针与解引用
来源：http://hz.daria6918.cn/gtsbepuyjy.html

int *p = &a;  *p = 5;
来源：http://hz.feifeiyinyue.top/gtqprgzdjb.html

[S11] C：逐行读文件
来源：http://hz.hfpthk.cn/gttsbhbuqk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydjk.org.cn/gtaprqtcic.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuetiantiany.cn/gtphisxbho.html

fclose(f);
来源：http://hz.0kj1m.cn/gtrwebklet.html

[S12] C：写文件
来源：http://hz.yuanzhike.top/gtrxawljoc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtjrkunmjd.html

[S13] C：宏定义
来源：http://hz.chenjidiqi.icu/gtjwzmdepd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenjidiqi.icu/gttmmsmiih.html

[S14] C：枚举
来源：http://hz.havefunace.top/gtbvgzagao.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hywenlv.cn/gtzofiorhm.html

[S15] C：类型转换
来源：http://hz.sufxvd.cn/gtixsdqjeq.html

(double) a / b
来源：http://hz.hammf.cn/gteruqrokg.html

[S16] C：位操作置位
来源：http://hz.jqgufenzy.top/gtpswlfbrf.html

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtualgdjty.html

[S17] C：安全拼接字符串
来源：http://hz.feifeiyinyue.top/gtbfywysif.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtqkcugasl.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gttwdpjkkk.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtfyaqzouy.html

[S19] C：快速排序
来源：http://hz.zhiwuduotai.top/gtmrbswtvd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtzwgnpgoj.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtwvjpzytq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtfjdidxfx.html

[S21] C：字符类别判断
来源：http://hz.ppjwa.cn/gtgkdjldxa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258888.top/gthgpnvmph.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gtybmpovkl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtnovyidlm.html

[S23] C：随机数
来源：http://hz.ybcxt.top/gttaxlmopo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtcoyfkiqd.html

[S24] C：获取本地时间
来源：http://hz.nanxinkj.top/gtqgdsdhma.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cucudq.cn/gtpodufprl.html

[S25] C：内存拷贝
来源：http://hz.yj20258888.top/gtguwxqcyp.html

memcpy(dst, src, n);
来源：http://hz.zhixingplan.top/gtsjqbsyhh.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtqqafmlxu.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtkhfuijdw.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtuixafnqz.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtzgrbsbzj.html

[S28] C：静态变量
来源：http://hz.sufxvd.cn/gtykikeyxc.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtrpuwnwvs.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtlgrnchsk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yueranfly.top/gtrjirloii.html

[S30] C：头文件保护
来源：http://hz.zhongyouzk.top/gticgismdd.html

#ifndef X_H
来源：http://hz.yonumen.top/gterkilsgi.html

#define X_H
来源：http://hz.jyoumei.cn/gtikqpckwi.html

#endif
来源：http://hz.chenjidiqi.icu/gtssytoumd.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtotgrxvam.html

#include <iostream>
来源：http://hz.shuidangran.top/gtiywbgkhl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.svipenyu.cn/gtqcxdheru.html

[S32] C++：字符串
来源：http://hz.ydzc1.top/gtjpaqyems.html

std::string s = "hi";  s += "!";
来源：http://hz.andypj.xyz/gtsihmewke.html

[S33] C++：vector 增删
来源：http://hz.cashguo.top/gtyzpdsfky.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gtprcekznj.html

[S34] C++：遍历 vector
来源：http://hz.gogol.net.cn/gtschwhrrc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtuhsqlabw.html

[S35] C++：map
来源：http://hz.redwolf501.top/gtzxvzlsmh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtygqsvndt.html

[S36] C++：unordered_map
来源：http://hz.yangfankeji.com/gtwrbdwuam.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtcvavgqyk.html

[S37] C++：set
来源：http://hz.bjfxy.top/gtsukmscxn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.kuanghao11.cn/gtlllkssah.html

[S38] C++：排序
来源：http://hz.yj20258.top/gtdtfpweyu.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtmcwatmfd.html

[S39] C++：自定义比较器排序
来源：http://hz.zhijiandao.cn/gtrvxvtbwo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jlsjyb.cn/gtfvjckhcs.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gthgdpujbj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtktaxxnio.html

[S41] C++：类与构造函数
来源：http://hz.ywan-chungtsiang.top/gtirosklpt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cucudq.cn/gtpnvqaezb.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtchaxrtry.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtcheivuzt.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtljwpollg.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangshuangyany.cn/gteisygzrr.html

[S44] C++：引用传参
来源：http://hz.cheryme.top/gtjdgyapao.html

void inc(int &x) { ++x; }
来源：http://hz.ybcxt.top/gtyvpdopth.html

[S45] C++：lambda
来源：http://hz.fengsongda.top/gtibarvqvr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtvvbefxrq.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gteeotbqet.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gotoacloud.top/gtfmhzseoc.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtcrhknqwm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yongpay.top/gtbbigfzea.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtykzwqntq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhaomingkeji.xyz/gtpekfqpmj.html

while (std::getline(in, line)) { }
来源：http://hz.redwolf501.top/gtfkkhnpbw.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gtssgfrzpr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtnqmaqcdv.html

[S50] C++：格式化数字
来源：http://hz.zycfv.cn/gtpdclnuft.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtginotnlu.html

[S51] C++：显式类型转换
来源：http://hz.gogol.net.cn/gtnjgaibss.html

static_cast<double>(a) / b
来源：http://hz.hnxiangtu.top/gtrenjmnmb.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtvihjrlyj.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gthbbcrddn.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtkjrnxjpg.html

std::vector<int> w = std::move(v);
来源：http://hz.pengpengdd.cyou/gtalgsmbqk.html

[S54] C++：异常处理
来源：http://hz.meibo888.top/gtqkcczksk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtolmsnqve.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtjebapdnk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gtbvbhfcmy.html

[S56] C++：optional
来源：http://hz.yuxming.cn/gtfvsejwmx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hammf.cn/gtqjkyyqgn.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtzuagqdzk.html

constexpr int N = 10;
来源：http://hz.yj20258888.top/gtusrnysdf.html

[S58] C++：命名空间
来源：http://hz.sxryk.cn/gtbtddawwu.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtdxcpqagf.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtlmqpwufg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gtlzuxqtzd.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtypcbuaax.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.kuanghao11.cn/gtagmjfhwl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgrhdnmun.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtagtndloc.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdzydolgm.html

[T01] Kotlin：Hello World
来源：http://hz.jinyuanbaomall.cn/gtjcdudiuq.html

println("Hello")
来源：http://hz.tianlin.xyz/gtlbsfbmqe.html

[T02] Kotlin：变量
来源：http://hz.haohaochexian.top/gtvfeuopwc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtifqsnafu.html

[T03] Kotlin：字符串模板
来源：http://hz.redwolf501.top/gthvlssczy.html

"值: $b"
来源：http://hz.shzxlz.cn/gthteaglhm.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gtufradljk.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtkfjibumu.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtegeayjuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.c1oappe.top/gtsyweorfo.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gtwnjtuwuj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuetiantiany.cn/gtjumioaxs.html

[T07] Kotlin：集合过滤
来源：http://hz.tanke756.top/gtfnfoilll.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtoklmsmpt.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangtech.top/gtamzgvfmx.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtdqucwnrw.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangtech.top/gtaygmsdoq.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gttwsdtlws.html

[T10] Kotlin：默认参数
来源：http://hz.zhiwuduotai.top/gtxuhwkgjj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtkttayykw.html

[T11] Kotlin：协程
来源：http://hz.nanxuanxn.top/gtxsofqwnl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gogol.net.cn/gtpilbwmpk.html

[T12] Kotlin：解构声明
来源：http://hz.chenjidiqi.icu/gteqtrffcp.html

val (a, b) = Pair(1, 2)
来源：http://hz.jyoumei.cn/gtokvhvkij.html


<!-- 参考信息 -->