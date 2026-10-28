代发 wailian999

esac
来源：http://hz.c1oappe.top/gtsmicyepl.html

[R12] for 遍历文件
来源：http://hz.yuxming.cn/gtlxjcmgqe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gteitygjdj.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtvmqdjbhi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtrfprjngo.html

[R14] C 风格 for
来源：http://hz.snrcjt.cn/gtsarqvqmk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gtjdpvfwrq.html

[R15] while 逐行读文件
来源：http://hz.zhengqikj.top/gtoxpbbdyp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtvupilhlx.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtwiwkzhii.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtpzdaqcnq.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtclsojtoa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.snrcjt.cn/gtumjziltm.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtazfnfjmu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yueranfly.top/gtzytbqmfj.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtypdydelz.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gtqyifkgvt.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtyeveoqoa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtvoodxwla.html

[R21] 字符串长度
来源：http://hz.zhaomingkeji.xyz/gtakdzdaop.html

echo "${#s}"
来源：http://hz.nwbrower.top/gtmejtpsci.html

[R22] 截取子串
来源：http://hz.yanxiufei.cn/gtubgupoax.html

echo "${s:0:5}"
来源：http://hz.nanxinkj.top/gtnwpvlkik.html

[R23] 字符串替换
来源：http://hz.yonumen.top/gtimhukfyu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnqzz.top/gtqraxgipt.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gttzesstvj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtgchsoabn.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtpimfeaad.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj202588.top/gtsmspxkel.html

[R26] 命令替换
来源：http://hz.svipenyu.cn/gteyamtbpk.html

now=$(date +%F); echo "$now"
来源：http://hz.daria6918.cn/gtdsbiyjib.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtobpcfehs.html

echo $((1 + 2 * 3))
来源：http://hz.gogol.net.cn/gtpryghzaq.html

[R28] 浮点运算
来源：http://hz.hysaishi.cn/gtqfzxdfpu.html

echo "scale=2; 10/3" | bc
来源：http://hz.pycfn.com/gtmzmwhjbp.html

[R29] 定义函数
来源：http://hz.jqgufenzy.top/gtvlnkxnnv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.quarkkingdee.top/gtpdsudpmr.html

[R30] 函数返回状态码
来源：http://hz.redwolf501.top/gtebfnqftw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gtpjdzjmlc.html

[R31] 局部变量
来源：http://hz.haohaochexian.top/gtwqauogmd.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgufenzy.top/gtgehrqohg.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtsnbpqkqp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tianlin.xyz/gtlpobjgtv.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtezrjjfwk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sysykeji.top/gtuzirdflh.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtrdzsipmg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtluapizvy.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtxdeimdyj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydzc1.top/gtxyhyszlb.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtlempcwlq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.wangdashe.top/gtfzkmnenx.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtrdknddvc.html

files=$(ls -1)
来源：http://hz.gotoacloud.top/gtcdwcodzj.html

[R38] 管道串联
来源：http://hz.cdnleiting.top/gteeydwlgo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xylfe.cn/gtkuaqfenf.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgufenzy.top/gtqayvqlah.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtamrxzkau.html

[R40] 追加写日志
来源：http://hz.shzxlz.cn/gtjqfoobdd.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtjqetjyjp.html

[R41] 丢弃输出
来源：http://hz.yvedp.cn/gtmjbacybe.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gtulhrdyva.html

[R42] 输入重定向
来源：http://hz.yuxming.cn/gtyskpuscm.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtrsndzyis.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtcfnrjttc.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gtkuljejjq.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtzsdmlgfc.html

find . -mtime -7 -type f
来源：http://hz.cashguo.top/gtchuacuez.html

[R45] 批量删除
来源：http://hz.yj20258.top/gtqpdfltrh.html

find . -name "*.tmp" -delete
来源：http://hz.jqgfzy.top/gtmwfyqzfe.html

[R46] 递归替换文件内容
来源：http://hz.xylfe.cn/gtbqtytgih.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtvnzrhcam.html

[R47] sed 单行替换
来源：http://hz.zhijiandao.cn/gtxnqdowgk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pycfn.com/gtmxztzsax.html

[R48] awk 取指定列
来源：http://hz.zhiwuduotai.top/gtneiexzts.html

awk '{print $1, $3}' a.txt
来源：http://hz.redwolf501.top/gtxwpfyjfg.html

[R49] awk 带条件
来源：http://hz.guowangkeji.top/gtkxiegncw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtlmlqtsob.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gtxjeqbbul.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtjnvfrzvx.html

[R51] 排序去重取前几
来源：http://hz.chenlongwang.top/gtbzhsybze.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.mhx1999.top/gtsdmqdyui.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtqqqnbqua.html

wc -l a.txt
来源：http://hz.jinyuanbaomall.cn/gtovbsmlnz.html

[R53] 查看文件头与实时尾
来源：http://hz.shzxlz.cn/gtvoepamkx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gtsupiysip.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtwgdgaixg.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gttnzutuhj.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gthsqoflmo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.haohaochexian.top/gtiletpwwo.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangtech.top/gtwspgafjh.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gtzctqfnvq.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtxyfeqegp.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gttgwjjgoi.html

[R58] 下载文件
来源：http://hz.nwbrower.top/gtxklknwgf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gttyagilno.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtrzihuxfu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zycfv.cn/gttmazeyxt.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtujroomhb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cqqwz.cn/gtjntnvjyj.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangkeji.top/gtlctvpozv.html

df -h;  du -sh *
来源：http://hz.snrcjt.cn/gtotatgvav.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtsujpxawe.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gtwhtzhefy.html

[R63] 内存与进程
来源：http://hz.zhengqikj.top/gtnjxgdnws.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gtixjjbhmz.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtypjlxzfj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shuidangran.top/gtqawzfixi.html

[R65] 查看端口占用
来源：http://hz.gzhubu.top/gtzioxnzqx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtgpyhsjmk.html

[R66] 定时任务
来源：http://hz.xuetiantiany.cn/gtodlgrzya.html

crontab -e;  crontab -l
来源：http://hz.aibaodan.cn/gtjitqvquz.html

[R67] 生成随机十六进制串
来源：http://hz.xuetiantiany.cn/gtxkwhndby.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gteunqedfm.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtkebijfmx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenzaomai.com/gtxktmosvk.html

[R69] 生成随机密码
来源：http://hz.ybcxt.top/gtoeimlqgv.html

head -c 16 /dev/urandom | base64
来源：http://hz.cucudq.cn/gtcooeztxg.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtlrfouxfh.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtctwwmufl.html

[R71] 日期格式化
来源：http://hz.zhoulong.xyz/gttkjonejv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.haohaochexian.top/gtmbxuyico.html

[R72] 等待端口就绪
来源：http://hz.sufxvd.cn/gtythydean.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guannengcc.top/gtjndmbuxx.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtublmkwiq.html

split -l 1000 big.log part_
来源：http://hz.hywenlv.cn/gtjbcrspjr.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtjzusmjsz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cheryme.top/gtqjtobfyh.html

[R75] 导出环境变量
来源：http://hz.birdmap.top/gtkbofhwkl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtooonnsqi.html

[R76] 使用临时文件
来源：http://hz.hywenlv.cn/gtracrkwgq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtixxxxmeo.html

[R77] 读取用户输入
来源：http://hz.zdqjudy.top/gtqyqepzys.html

read -rp "请输入: " ans
来源：http://hz.ppjwa.cn/gtgiruhtzd.html

[R78] 交互式菜单
来源：http://hz.chenlongwang.top/gtzbbbvaye.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.vqdsnc.cn/gtsfdsylyw.html

[R79] 解析命令行选项
来源：http://hz.nanxuanxn.top/gtflwansyj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dianchejie.cn/gtxkjdvsnh.html

[R80] 查看脚本执行耗时
来源：http://hz.dashuyun.cn/gtdkxxzvoj.html

time ./run.sh
来源：http://hz.guannengcc.top/gtvbzjhwsq.html

================================================================================
来源：http://hz.aibaodan.cn/gtuwrccjns.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtdxzkkbcx.html

================================================================================
来源：http://hz.hywenlv.cn/gtobskdaas.html

[S01] C：Hello World
来源：http://hz.xuetiantiany.cn/gtpulytyvk.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gthhgmvfio.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hammf.cn/gtpmqsvthu.html

[S02] C：变量与格式化输出
来源：http://hz.gzhubu.top/gtgdsnwvbs.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gthciyypmi.html

[S03] C：读入整数
来源：http://hz.quarkkingdee.top/gtdnrtpfrj.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtxskemuqp.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangkeji.top/gttbbxlqol.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangkeji.top/gtfenyzged.html

[S05] C：字符串长度
来源：http://hz.zycfv.cn/gtuwomdong.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtnwrvfscu.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtkevttjwq.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtnzpdfltu.html

[S07] C：数组遍历求和
来源：http://hz.svipenyu.cn/gtgdylxwic.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtcxuwoyhx.html

[S08] C：动态内存分配与释放
来源：http://hz.hongshengwenyu.top/gteicjeqeq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ehwqpu.com/gticvsfhrh.html

[S09] C：结构体定义与初始化
来源：http://hz.yongpay.top/gtlwuqsgwz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuanzx.com/gtmmohyvrn.html

[S10] C：指针与解引用
来源：http://hz.xuanzx.com/gttkwwqwxv.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtmlerylbg.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtyqboltlz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtaurvlbdk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigfzy.top/gtsqwynoce.html

fclose(f);
来源：http://hz.andypj.xyz/gtjyhpgwuf.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gtqarghgnb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ybcxt.top/gtgjfgpfpi.html

[S13] C：宏定义
来源：http://hz.ybcxt.top/gtdengwart.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.kuanghao11.cn/gtiqjxpjru.html

[S14] C：枚举
来源：http://hz.guannengcc.top/gtpffslbau.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shuidangran.top/gtobwdarbe.html

[S15] C：类型转换
来源：http://hz.ivvv.top/gtegxqjpzm.html

(double) a / b
来源：http://hz.316326.xyz/gtuakwhfgt.html

[S16] C：位操作置位
来源：http://hz.zhiwuduotai.top/gtclbyvssx.html

x |= (1 << 3);
来源：http://hz.chenzaomai.com/gtyutpeocb.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtfwdawwct.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenjidiqi.icu/gtbtnmponm.html

[S18] C：命令行参数
来源：http://hz.redwolf501.top/gtltclgffn.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtrzfnqayd.html

[S19] C：快速排序
来源：http://hz.jinghuilouyu.cn/gtmcvclbhi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtxplguwka.html

[S20] C：二分查找
来源：http://hz.ydzc1.top/gtcbfquobr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gteloywjzy.html

[S21] C：字符类别判断
来源：http://hz.xylfe.cn/gtvwrjsdne.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tanke756.top/gthtqrypby.html

[S22] C：字符串转数字
来源：http://hz.chenlongwang.top/gtckwjyoth.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gtzeyxyjng.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtdpfccvph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtpxyfcoak.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtunlkqihs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hysaishi.cn/gtveylyhie.html

[S25] C：内存拷贝
来源：http://hz.gzhubu.top/gtozmtklir.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gtbshimldo.html

[S26] C：内存清零
来源：http://hz.yj20258888.top/gtyommyhyn.html

memset(a, 0, sizeof a);
来源：http://hz.nanxuanxn.top/gtkafifbto.html

[S27] C：定义常量
来源：http://hz.jlsjyb.cn/gtiumugilz.html

const double PI = 3.14159;
来源：http://hz.wangdashe.top/gtosncinqg.html

[S28] C：静态变量
来源：http://hz.hywenlv.cn/gtnmlvhscz.html

static int counter = 0;
来源：http://hz.bjfxy.top/gtpwolqjtz.html

[S29] C：变参函数
来源：http://hz.ywan-chungtsiang.top/gtypltkxwb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jlsjyb.cn/gtzobqjuld.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtvxzqlizy.html

#ifndef X_H
来源：http://hz.c1oappe.top/gtcafcwhbp.html

#define X_H
来源：http://hz.andypj.xyz/gtutiptzeq.html

#endif
来源：http://hz.aizwys.cn/gtgjxllvpx.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtxurblgnm.html

#include <iostream>
来源：http://hz.bjfxy.top/gtbyafyxpo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.havefunace.top/gtqbbsiwod.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtahedvzvo.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gtkzjiopji.html

[S33] C++：vector 增删
来源：http://hz.ivvv.top/gttxtoeksb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtxnuoapye.html

[S34] C++：遍历 vector
来源：http://hz.jianghu66.top/gtkkigqzyg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtficpugpu.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtwbmcecyn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtkcsqluzp.html

[S36] C++：unordered_map
来源：http://hz.cucudq.cn/gtwwbfjkrf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtbzgesfdx.html

[S37] C++：set
来源：http://hz.cqqwz.cn/gtgxtahrna.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jiagoushi.top/gtmpuooyqa.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtveipaxbw.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gtglimidpa.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gtntsvcybq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgfzy.top/gtnftsfdqe.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtprwhsrzm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtfirmtgtm.html

[S41] C++：类与构造函数
来源：http://hz.52xcode.cn/gtssmeruyw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gtgkifqwmg.html

[S42] C++：继承与虚函数
来源：http://hz.cdnleiting.top/gthdnjzfqn.html

class B : public Base { public: void f() override {} };
来源：http://hz.vqdsnc.cn/gtxlvevgyk.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtmpzugwfz.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtzrbcyupt.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtpxveanwv.html

void inc(int &x) { ++x; }
来源：http://hz.redwolf501.top/gtxghzjfqi.html

[S45] C++：lambda
来源：http://hz.jinqigfzy.top/gthqhdombw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtyjhklfnj.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtzlstnfeu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtrzwgsyje.html

[S47] C++：结构化绑定遍历
来源：http://hz.redwolf501.top/gtdkhzszic.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtyptnmjec.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gtfghlwvgf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuetiantiany.cn/gtwhhvxlal.html

while (std::getline(in, line)) { }
来源：http://hz.iojbl.cn/gtnupsvrbb.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtonvdikek.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.havefunace.top/gtekshifnd.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gttgsgvqfp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ppjwa.cn/gttadwnqef.html

[S51] C++：显式类型转换
来源：http://hz.meibo888.top/gtgdhbhhod.html

static_cast<double>(a) / b
来源：http://hz.jlsjyb.cn/gtmhydpyht.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtwcpwngcu.html

int size() const noexcept { return n_; }
来源：http://hz.yonumen.top/gtunxigqsp.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangkeji.top/gtxeybnzbw.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gtinbfkozj.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gtssjadoyf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangshuangyany.cn/gtcgigaync.html

[S55] C++：结构化绑定
来源：http://hz.tian-w.cn/gtrhgetikw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guowangkeji.top/gtbudgyzdm.html

[S56] C++：optional
来源：http://hz.shangyingyoupin.top/gtmdzcsxgt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj202588.top/gthycqpjff.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtufwnegou.html

constexpr int N = 10;
来源：http://hz.jyoumei.cn/gtnqfssgjp.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtijuzporh.html

namespace ns { int f() { return 1; } }
来源：http://hz.jiagoushi.top/gtblibfaze.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gttojufsew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnxiangtu.top/gtqtdnuqsj.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gttxpdjqpn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.feifeiyinyue.top/gtgslicpts.html

================================================================================
来源：http://hz.hnxiangtu.top/gtoaqkurhq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.svipenyu.cn/gttnlxxwvm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdmdkkjil.html

[T01] Kotlin：Hello World
来源：http://hz.vqdsnc.cn/gtbkjoerom.html

println("Hello")
来源：http://hz.sysykeji.top/gtrgabjsug.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtmtgkbbzy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigfzy.top/gtabkavmdm.html

[T03] Kotlin：字符串模板
来源：http://hz.cqqwz.cn/gtcnmtpwfg.html

"值: $b"
来源：http://hz.haohaochexian.top/gtunbpqdjj.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtbacwtbiz.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtyhuxwroi.html

[T05] Kotlin：when 表达式
来源：http://hz.yangfankeji.com/gtpfmerbbt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.birdmap.top/gthftodlnj.html

[T06] Kotlin：集合映射
来源：http://hz.gogol.net.cn/gtgphcwgcn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangtech.top/gttevnxaej.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtdtkfdauc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhongyouzk.top/gtdwyxzvil.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtsltautef.html

data class User(val name: String, val age: Int)
来源：http://hz.aizwys.cn/gtwkktekpd.html

[T09] Kotlin：扩展函数
来源：http://hz.sxryk.cn/gtrbvemfje.html

fun String.exclaim() = this + "!"
来源：http://hz.feifeiyinyue.top/gttdlksphl.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gtmxfxdebh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigufen.top/gtymulchdg.html

[T11] Kotlin：协程
来源：http://hz.zhijiandao.cn/gtryieahuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shzxlz.cn/gtwflzbaaj.html

[T12] Kotlin：解构声明
来源：http://hz.ydjk.org.cn/gtfsrghccc.html

val (a, b) = Pair(1, 2)
来源：http://hz.cdnleiting.top/gtvrtsreak.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigufen.top/gttyuesfld.html

val m = mapOf("a" to 1)
来源：http://hz.chenjidiqi.icu/gtmyekdchr.html

[T14] Kotlin：循环
来源：http://hz.hammf.cn/gtykbbovlw.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtgvbsactu.html


<!-- 参考信息 -->