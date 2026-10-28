代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtkrgqcjlm.html

[R14] C 风格 for
来源：http://hz.mhx1999.top/gtskyiggod.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtbmyboqgs.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtlovufyac.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tian-w.cn/gtoverzmlk.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gtrlapiqbt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtwhprzzfd.html

[R17] 数组定义与取值
来源：http://hz.jiagoushi.top/gthwaqlrvm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gtvvgoljxr.html

[R18] 遍历数组
来源：http://hz.ivvv.top/gtisacghnb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.bjfxy.top/gtmmknjclk.html

[R19] 数组长度
来源：http://hz.meibo888.top/gtbvhktkxt.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtaaooyfwb.html

[R20] 关联数组（字典）
来源：http://hz.yueranfly.top/gtgyebcxop.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenjidiqi.icu/gtiisamvsr.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtmbgjlrwt.html

echo "${#s}"
来源：http://hz.daxiang520.top/gtzzniohoy.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtccqwvgck.html

echo "${s:0:5}"
来源：http://hz.c1oappe.top/gthqanikls.html

[R23] 字符串替换
来源：http://hz.hammf.cn/gtwxgmnagg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yangfankeji.com/gtpgvtaqlw.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtksmptvoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtwimarvlu.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtereocwja.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtvlzjbpuq.html

[R26] 命令替换
来源：http://hz.guannengcc.top/gtpkldffhq.html

now=$(date +%F); echo "$now"
来源：http://hz.ppjwa.cn/gtowwkhutu.html

[R27] 算术展开
来源：http://hz.redwolf501.top/gtkcslxobg.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtefydbopb.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtsisotsrg.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtpjfmligj.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtbwlxatxx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtusrqxhti.html

[R30] 函数返回状态码
来源：http://hz.9152youxi.cn/gtjxvmrtso.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gtkbtsrfzz.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtnxcladth.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigfzy.top/gtbblnazql.html

[R32] 参数个数校验
来源：http://hz.vqdsnc.cn/gtuzjyhufb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtxkpqbneh.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtwccqepof.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gttqxidcfo.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtzyqdwtbz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtivgollfi.html

[R35] 后台执行并等待
来源：http://hz.pycfn.com/gtafxrzyjh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.iojbl.cn/gtfsfusnwr.html

[R36] 并发执行多个任务
来源：http://hz.svipenyu.cn/gttkztqivf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xinyue.icu/gtterupnwi.html

[R37] 把输出赋给变量
来源：http://hz.shangyingyoupin.top/gtbjwlwicn.html

files=$(ls -1)
来源：http://hz.aibaodan.cn/gtcjemqtvr.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtjewzdhcf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jiagoushi.top/gtyyvuuoxu.html

[R39] 重定向标准输出与错误
来源：http://hz.quarkkingdee.top/gtxzrtoyue.html

cmd > out.log 2>&1
来源：http://hz.yj202588.top/gtkuwgoxxt.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtbixmates.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gthjgdbplp.html

[R41] 丢弃输出
来源：http://hz.feifeiyinyue.top/gttwpocyyq.html

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gtdihcmldq.html

[R42] 输入重定向
来源：http://hz.meibo888.top/gtvpkwathe.html

wc -l < a.txt
来源：http://hz.ehwqpu.com/gttlmdwquq.html

[R43] 按名字查找文件
来源：http://hz.hammf.cn/gteqecwxxs.html

find . -name "*.log" -type f
来源：http://hz.jiagoushi.top/gtegdyhnjb.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gtmsrimcwp.html

find . -mtime -7 -type f
来源：http://hz.jqgfzy.top/gtgtvptlqf.html

[R45] 批量删除
来源：http://hz.andypj.xyz/gtmffvxrxt.html

find . -name "*.tmp" -delete
来源：http://hz.smart0.xyz/gtjkwzhsoq.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtnneplqfq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gtltxpijav.html

[R47] sed 单行替换
来源：http://hz.shzxlz.cn/gttatcmgrk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigfzy.top/gteqefbzeq.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtttdswhku.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtefqhgjaa.html

[R49] awk 带条件
来源：http://hz.gzhubu.top/gtqkxyxwfx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtcmhivysv.html

[R50] awk 求和
来源：http://hz.hysaishi.cn/gtfhzhnhho.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtscpvuzjq.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtuvmuhzsr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtoetpvatp.html

[R52] 统计行数
来源：http://hz.daxiang520.top/gtssgurbzd.html

wc -l a.txt
来源：http://hz.feifeiyinyue.top/gtvekelrry.html

[R53] 查看文件头与实时尾
来源：http://hz.birdmap.top/gtwtgbktrh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtefkuxkse.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtveigclue.html

diff a.txt b.txt
来源：http://hz.shuidangran.top/gtmnuwvyli.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gttfjbiijs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gtiztfisis.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtvvycitmf.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtsvgaucpj.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtnjbrbimj.html

ssh user@host 'uptime'
来源：http://hz.ywan-chungtsiang.top/gtwhnrucfc.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtiscxgowz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gtrpoizefa.html

[R59] 发 POST JSON
来源：http://hz.jqgufenzy.top/gtsrainzui.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtmlmdhcyy.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gteazolfeh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenlongwang.top/gtwbofashm.html

[R61] 磁盘占用
来源：http://hz.xziqi.cn/gtriakyvss.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gttjfudurb.html

[R62] 找最占空间的文件
来源：http://hz.zdqjudy.top/gtaienwwaa.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtokqpospv.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtgicxwujt.html

free -h;  ps aux | grep nginx
来源：http://hz.hywenlv.cn/gtmhhhdmpz.html

[R64] 结束进程
来源：http://hz.fengsongda.top/gtmypsmqef.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jianghu66.top/gtkrymvsug.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtegopmdfu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtsgltbvdt.html

[R66] 定时任务
来源：http://hz.xziqi.cn/gtjsqdtpwu.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtazmitrlc.html

[R67] 生成随机十六进制串
来源：http://hz.shzxlz.cn/gtixdrythz.html

openssl rand -hex 16
来源：http://hz.zhengqikj.top/gtgcuiqzdz.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtvqjhdpoc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtbgcviopd.html

[R69] 生成随机密码
来源：http://hz.gotoacloud.top/gtszkiktza.html

head -c 16 /dev/urandom | base64
来源：http://hz.xziqi.cn/gtmdkczinz.html

[R70] 时间戳与互转
来源：http://hz.meibo888.top/gtqjrxjywo.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtqhslwnye.html

[R71] 日期格式化
来源：http://hz.jqgfzy.top/gtnprhvadh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinyuanbaomall.cn/gtypinyqkc.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gtzlepkgie.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xylfe.cn/gtwlalpjvq.html

[R73] 分割大日志
来源：http://hz.wangdashe.top/gtejylhsim.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtupymdljq.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtzcanrzyi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtsbqupzwz.html

[R75] 导出环境变量
来源：http://hz.nanxuanxn.top/gtmerifgxr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhoulong.xyz/gtuqrxrlkx.html

[R76] 使用临时文件
来源：http://hz.hysaishi.cn/gtftavmfks.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtmvdulxnu.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtzrsoiaxr.html

read -rp "请输入: " ans
来源：http://hz.fengsongda.top/gtyafufwty.html

[R78] 交互式菜单
来源：http://hz.ywan-chungtsiang.top/gtrniafyzo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gtweuqgnvz.html

[R79] 解析命令行选项
来源：http://hz.nanxuanxn.top/gtllizofpn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gtjwayvpet.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigfzy.top/gthlexykpx.html

time ./run.sh
来源：http://hz.guowangkeji.top/gtxblksfle.html

================================================================================
来源：http://hz.gaohongyu789.top/gtzstpemnh.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtycixtmkd.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrgztvaho.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtywjlgvzb.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtkphalmwq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gtjfsmsala.html

[S02] C：变量与格式化输出
来源：http://hz.cqqwz.cn/gteyshurgk.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtvvsfjrok.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtdwcjlynq.html

int x; scanf("%d", &x);
来源：http://hz.cashguo.top/gtfoqopssj.html

[S04] C：字符串复制
来源：http://hz.tianlin.xyz/gtacjkgesc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ivvv.top/gtufhvqqfk.html

[S05] C：字符串长度
来源：http://hz.birdmap.top/gtstyigbrv.html

strlen(s)
来源：http://hz.jianghu66.top/gtqcwmedhy.html

[S06] C：字符串比较
来源：http://hz.ydzc1.top/gtczivehee.html

strcmp(a, b) == 0
来源：http://hz.chenlongwang.top/gtsmeikjlw.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtfpauxqlc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtheujrvll.html

[S08] C：动态内存分配与释放
来源：http://hz.zhixingplan.top/gtuunzpful.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gtuciaghoq.html

[S09] C：结构体定义与初始化
来源：http://hz.hnxiangtu.top/gtyvyfookv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuxming.cn/gtyvyyeafl.html

[S10] C：指针与解引用
来源：http://hz.yueranfly.top/gtbqttzsdr.html

int *p = &a;  *p = 5;
来源：http://hz.xziqi.cn/gtztnwaoin.html

[S11] C：逐行读文件
来源：http://hz.yvedp.cn/gtfxyimlwt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtbkrmypui.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtrigydhnq.html

fclose(f);
来源：http://hz.aibaodan.cn/gtoegsqcfx.html

[S12] C：写文件
来源：http://hz.tianlin.xyz/gtsrhaxtxr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.snrcjt.cn/gtpcwqhixk.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtllvdqrgg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gtyswrcdpt.html

[S14] C：枚举
来源：http://hz.jlsjyb.cn/gtukinhcxc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.52xcode.cn/gthkccatll.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtmkqjmvab.html

(double) a / b
来源：http://hz.jinqigufen.top/gtpafkoadh.html

[S16] C：位操作置位
来源：http://hz.sxryk.cn/gtofzeuyvw.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtfwmqeazu.html

[S17] C：安全拼接字符串
来源：http://hz.tianlin.xyz/gtpjqhpcmy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtxwtjwayz.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtiupwzmpr.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtksqlllkb.html

[S19] C：快速排序
来源：http://hz.zhaomingkeji.xyz/gtwuwyzeca.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtlwfqrynz.html

[S20] C：二分查找
来源：http://hz.dashuyun.cn/gtbblkclfo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtlyudieaw.html

[S21] C：字符类别判断
来源：http://hz.snrcjt.cn/gtmwcwerkp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cheryme.top/gtzsbcsfyl.html

[S22] C：字符串转数字
来源：http://hz.zycfv.cn/gtrqjwldvc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gthgdhokar.html

[S23] C：随机数
来源：http://hz.snrcjt.cn/gtilushejv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gtwemeruyo.html

[S24] C：获取本地时间
来源：http://hz.zhixingplan.top/gtfypvsdbc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fzhhl.top/gtrcxdcaeb.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtkodygtgm.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangtech.top/gtmoehosus.html

[S26] C：内存清零
来源：http://hz.yanxiufei.cn/gthklqoeva.html

memset(a, 0, sizeof a);
来源：http://hz.yanxiufei.cn/gtyeqzdvrx.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtcgsiflut.html

const double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtycdpncog.html

[S28] C：静态变量
来源：http://hz.andypj.xyz/gteyspcbvz.html

static int counter = 0;
来源：http://hz.yj20258888.top/gtiuxoiiba.html

[S29] C：变参函数
来源：http://hz.zhixingplan.top/gtxtjatvni.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgufenzy.top/gtklzypxbn.html

[S30] C：头文件保护
来源：http://hz.jinyuanbaomall.cn/gtohbkqbrw.html

#ifndef X_H
来源：http://hz.birdmap.top/gtnrmdncxd.html

#define X_H
来源：http://hz.daxiang520.top/gtkqlxpqby.html

#endif
来源：http://hz.cucudq.cn/gtqkidfcde.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtslkxkdnp.html

#include <iostream>
来源：http://hz.cheryme.top/gtspeolgbu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.birdmap.top/gtuaxwaykc.html

[S32] C++：字符串
来源：http://hz.jqgfzy.top/gtkxeiiikr.html

std::string s = "hi";  s += "!";
来源：http://hz.yuxming.cn/gttrybcrzp.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtipfofnaj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydjk.org.cn/gtoeqdjttp.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtuiyuvomf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtzerxebqs.html

[S35] C++：map
来源：http://hz.cucudq.cn/gtacpfeqyk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtvsuplbls.html

[S36] C++：unordered_map
来源：http://hz.c1oappe.top/gtoeafdknd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtxfdoygfb.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtlnngtrfw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gthxuuraky.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtbprjqyfj.html

std::sort(v.begin(), v.end());
来源：http://hz.xuetiantiany.cn/gtacxviwxt.html

[S39] C++：自定义比较器排序
来源：http://hz.fengsongda.top/gtpiivamnc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gtiskvhodo.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtttiljvwq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtjkvdcnya.html

[S41] C++：类与构造函数
来源：http://hz.aibaodan.cn/gthohkyjxe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jianghu66.top/gthxqeqxjq.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtklhnesks.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtwjkdpuhc.html

[S43] C++：智能指针
来源：http://hz.wangshuangyany.cn/gtxceggidu.html

auto p = std::make_unique<int>(5);
来源：http://hz.jlsjyb.cn/gtltduqvmr.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangtech.top/gtqqducalz.html

void inc(int &x) { ++x; }
来源：http://hz.nwbrower.top/gtbptyzhsd.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gttliqrypj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigfzy.top/gtcnuflmff.html

[S46] C++：函数模板
来源：http://hz.zdqjudy.top/gtehuqehnl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinyuanbaomall.cn/gtoaigxczs.html

[S47] C++：结构化绑定遍历
来源：http://hz.pycfn.com/gtpcwznaep.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtmquxwlac.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtfjieemio.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhijiandao.cn/gtsdiwpsnt.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtsqxdimvc.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtiewwjfqv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenzaomai.com/gtgbryhgaq.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gtwerlfxvo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tanke756.top/gtbpnwywsp.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtnflytpgg.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtjqxympiz.html

[S52] C++：const 与 noexcept
来源：http://hz.xylfe.cn/gtjkhrqssv.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtcmrwymgz.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtdkxwxbrr.html

std::vector<int> w = std::move(v);
来源：http://hz.sufxvd.cn/gtnmsyqppk.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtqmeeqcgr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtluujousv.html

[S55] C++：结构化绑定
来源：http://hz.snrcjt.cn/gtbkjgglag.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aizwys.cn/gtsuxucmko.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtlqhkobcp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gotoacloud.top/gtfltbbhvn.html

[S57] C++：编译期常量
来源：http://hz.zhijiandao.cn/gtrbcawhuz.html

constexpr int N = 10;
来源：http://hz.hnqzz.top/gtiqkzwnxp.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gtiooydevs.html

namespace ns { int f() { return 1; } }
来源：http://hz.sxryk.cn/gtqhlinvsr.html

[S59] C++：静态断言
来源：http://hz.hongshengwenyu.top/gtjrfhwloc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.andypj.xyz/gtpgiuwrbd.html

[S60] C++：遍历并删除元素
来源：http://hz.shuidangran.top/gtjyljzqns.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtvaxkcyqe.html

================================================================================
来源：http://hz.9152youxi.cn/gtbpdzwwie.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gtjwmeqszs.html

================================================================================
来源：http://hz.hfpthk.cn/gtemwvrmni.html

[T01] Kotlin：Hello World
来源：http://hz.zhiwuduotai.top/gturctnutm.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtuxkmemha.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gttikltlbp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yonumen.top/gtrqcayxje.html

[T03] Kotlin：字符串模板
来源：http://hz.xingfuxueyuan.xyz/gtfkppujtb.html

"值: $b"
来源：http://hz.nanxuanxn.top/gtavhmienf.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtvbcmwptw.html

val n: String? = null;  n?.length
来源：http://hz.9152youxi.cn/gtgtonofvd.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gtgtbbshqn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gtrbpvtsbx.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gttmzlolhw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sxryk.cn/gtveqmnhfs.html

[T07] Kotlin：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtrhjlorba.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuetiantiany.cn/gtceoztmzp.html

[T08] Kotlin：数据类
来源：http://hz.jianghu66.top/gtroerybxz.html

data class User(val name: String, val age: Int)
来源：http://hz.yangfankeji.com/gtlqjjckhr.html

[T09] Kotlin：扩展函数
来源：http://hz.fzhhl.top/gtefzwiomr.html

fun String.exclaim() = this + "!"
来源：http://hz.fengsongda.top/gtoqayudru.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtjlixarcb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gtzxilhyme.html

[T11] Kotlin：协程
来源：http://hz.xingfuxueyuan.xyz/gtizyajzzy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtmtxknxoq.html

[T12] Kotlin：解构声明
来源：http://hz.zycfv.cn/gtixkhcefo.html

val (a, b) = Pair(1, 2)
来源：http://hz.tianlin.xyz/gtrymkkmko.html

[T13] Kotlin：只读 Map
来源：http://hz.xuetiantiany.cn/gtadvhgpxo.html

val m = mapOf("a" to 1)
来源：http://hz.yanxiufei.cn/gtkhdjccsl.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gtespculqf.html

for (i in 1..10) println(i)
来源：http://hz.smart0.xyz/gtuobpsscc.html

[T15] Kotlin：接口
来源：http://hz.c1oappe.top/gtpbwmfdpe.html

interface Shape { fun area(): Double }
来源：http://hz.cucudq.cn/gtgdrivbzk.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtabkoxpnb.html

print("Hello")
来源：http://hz.jlsjyb.cn/gtksquojfa.html


<!-- 参考信息 -->