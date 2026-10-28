代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtetcenidg.html

[R14] C 风格 for
来源：http://hz.chenlongwang.top/gtddrzcosz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shuidangran.top/gtusxjrhte.html

[R15] while 逐行读文件
来源：http://hz.fengsongda.top/gtwtezjouf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cdnleiting.top/gttkhgwwud.html

[R16] until 等待条件
来源：http://hz.yueranfly.top/gtckrpadlr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtvytzqguj.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtpmlrmoks.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jiagoushi.top/gtptmufeoo.html

[R18] 遍历数组
来源：http://hz.guowangkeji.top/gtjtbkaiso.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.feifeiyinyue.top/gtatevlxnn.html

[R19] 数组长度
来源：http://hz.nwbrower.top/gtmcxnkfnh.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gtszegfyda.html

[R20] 关联数组（字典）
来源：http://hz.pycfn.com/gtwpajbeck.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sufxvd.cn/gtcbdiagzw.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtizwahxax.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtuzjlebkx.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtkqimwzlt.html

echo "${s:0:5}"
来源：http://hz.wangdashe.top/gtqrbdxned.html

[R23] 字符串替换
来源：http://hz.zhiwuduotai.top/gthvmwdsuu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydjk.org.cn/gtkvonpmmk.html

[R24] 大小写转换
来源：http://hz.fzhhl.top/gtlaqrurcz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgfzy.top/gtghofpwrl.html

[R25] 去后缀 / 去前缀
来源：http://hz.jlsjyb.cn/gthqjqwmmi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xziqi.cn/gtnuxqivsw.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtogyesrgf.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtdizoezmi.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gtdaxcngiv.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtnlewbmlt.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtxadexcwa.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtnnnhurqe.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtllisynyz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtoeeetzgy.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtjmemnnem.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtafixxdcn.html

[R31] 局部变量
来源：http://hz.guowangkeji.top/gtbcggcixs.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhoulong.xyz/gtnfwzzixt.html

[R32] 参数个数校验
来源：http://hz.xuanzx.com/gtvtwgegky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtfyrkooxy.html

[R33] 捕获错误并提示行号
来源：http://hz.gzhubu.top/gtlrkrdkjq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgfzy.top/gtymbjvzob.html

[R34] 退出时清理
来源：http://hz.hnxiangtu.top/gtchkojzxj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtzhpjucpn.html

[R35] 后台执行并等待
来源：http://hz.xylfe.cn/gtwivjehbm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuanzhike.top/gtydayiify.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtmbrglxka.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gtejcpvqon.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtaslcmphz.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtnemjubpz.html

[R38] 管道串联
来源：http://hz.yonumen.top/gttomwhumh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenzaomai.com/gtlnteherd.html

[R39] 重定向标准输出与错误
来源：http://hz.haohaochexian.top/gttohqmlic.html

cmd > out.log 2>&1
来源：http://hz.xinyue.icu/gthqtazerj.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtshnzlvxo.html

echo "log" >> out.log
来源：http://hz.zhengqikj.top/gtdqqrbglv.html

[R41] 丢弃输出
来源：http://hz.redwolf501.top/gtzxgmtaky.html

cmd >/dev/null 2>&1
来源：http://hz.wangdashe.top/gtceunctyz.html

[R42] 输入重定向
来源：http://hz.yuxming.cn/gtuwbmzsgs.html

wc -l < a.txt
来源：http://hz.zhijiandao.cn/gtwfrjebdh.html

[R43] 按名字查找文件
来源：http://hz.xylfe.cn/gtjybksujj.html

find . -name "*.log" -type f
来源：http://hz.jlsjyb.cn/gtedthjsww.html

[R44] 按修改时间查找
来源：http://hz.nanxinkj.top/gtaeztpvvz.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gtesrevqeh.html

[R45] 批量删除
来源：http://hz.zycfv.cn/gtlsgozcdv.html

find . -name "*.tmp" -delete
来源：http://hz.vqdsnc.cn/gtatxjudfp.html

[R46] 递归替换文件内容
来源：http://hz.jianghu66.top/gtglmvbshu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ivvv.top/gtrqnvilqb.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtofssvuiu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cdnleiting.top/gtjnbalxvq.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtmwnlcwoo.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangdashe.top/gtjjmyhjlj.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gteyuurqxu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtsbfqykgf.html

[R50] awk 求和
来源：http://hz.cqqwz.cn/gtmlrfnqbj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nanxinkj.top/gtsqwvqbcn.html

[R51] 排序去重取前几
来源：http://hz.316326.xyz/gtnvpppioh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtuoqycszv.html

[R52] 统计行数
来源：http://hz.cucudq.cn/gttcdghhdh.html

wc -l a.txt
来源：http://hz.svipenyu.cn/gtgpentlvb.html

[R53] 查看文件头与实时尾
来源：http://hz.yuxming.cn/gtqzbcleng.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gzhubu.top/gtzovkdqqa.html

[R54] 比较两个文件
来源：http://hz.fzhhl.top/gtdossiraz.html

diff a.txt b.txt
来源：http://hz.c1oappe.top/gtefjemqaj.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gthqeyblvn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtxawnhtxm.html

[R56] 远程拷贝
来源：http://hz.fzhhl.top/gtmnltorzy.html

scp file user@host:/path/
来源：http://hz.cucudq.cn/gtxbjvlbup.html

[R57] 远程执行命令
来源：http://hz.yonumen.top/gtwjpzzuqy.html

ssh user@host 'uptime'
来源：http://hz.kuanghao11.cn/gtntphsyrl.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtaatsmttw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangshuangyany.cn/gtvzlroraj.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtzegxitrc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gogol.net.cn/gtpwoalzzg.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtrjcmjohl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtklwxmfpm.html

[R61] 磁盘占用
来源：http://hz.hnqzz.top/gtgylurpos.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtvbsswpcf.html

[R62] 找最占空间的文件
来源：http://hz.aizwys.cn/gtewhbdbot.html

du -ah . | sort -rh | head -10
来源：http://hz.jinghuilouyu.cn/gtzoekkvka.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gtpzqpfctq.html

free -h;  ps aux | grep nginx
来源：http://hz.yj202588.top/gtbifkegbs.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtlwvawtxf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cheryme.top/gtcqqfaxei.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gtmgdyqyaj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hywenlv.cn/gtuqdstell.html

[R66] 定时任务
来源：http://hz.smart0.xyz/gtjinhoixi.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtslygakti.html

[R67] 生成随机十六进制串
来源：http://hz.yanxiufei.cn/gtfihseqwy.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtwlcpbtkk.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtqtrxqyem.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gtbcbgwmky.html

[R69] 生成随机密码
来源：http://hz.snrcjt.cn/gtzzczpsdw.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigfzy.top/gtiylllipl.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gteirumhhs.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtvvdwupqy.html

[R71] 日期格式化
来源：http://hz.quarkkingdee.top/gtuhhrclkc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ywan-chungtsiang.top/gtwufiscey.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gttsgjtlrr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.meibo888.top/gtmsdghsct.html

[R73] 分割大日志
来源：http://hz.jlsjyb.cn/gtndpujmiv.html

split -l 1000 big.log part_
来源：http://hz.ppjwa.cn/gtwchtcevn.html

[R74] 批量重命名
来源：http://hz.tanke756.top/gtaacklbdu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sweek.top/gtocvamrqz.html

[R75] 导出环境变量
来源：http://hz.ydzc1.top/gtxcbenxjt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtqeylgdnb.html

[R76] 使用临时文件
来源：http://hz.andypj.xyz/gtqeeluhsn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtomjgnhbw.html

[R77] 读取用户输入
来源：http://hz.shzxlz.cn/gtkjfdpkvh.html

read -rp "请输入: " ans
来源：http://hz.xingfuxueyuan.xyz/gtttoslaxh.html

[R78] 交互式菜单
来源：http://hz.haohaochexian.top/gtrfqjcmub.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gttvhrmcsg.html

[R79] 解析命令行选项
来源：http://hz.fzhhl.top/gtqwpefxys.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xziqi.cn/gteiorzgyb.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtauxdkoqo.html

time ./run.sh
来源：http://hz.kuanghao11.cn/gtaenxsjjk.html

================================================================================
来源：http://hz.cheryme.top/gtjvjkmkph.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gthwwdvawl.html

================================================================================
来源：http://hz.zhixingplan.top/gttkezomci.html

[S01] C：Hello World
来源：http://hz.xinyue.icu/gtpsobdpvc.html

#include <stdio.h>
来源：http://hz.jiagoushi.top/gtvbgqttas.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxinkj.top/gtybxnvoyp.html

[S02] C：变量与格式化输出
来源：http://hz.zhoulong.xyz/gtcxuhvecl.html

int a = 10; printf("%d\n", a);
来源：http://hz.shzxlz.cn/gtyaefcuny.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtgrtlwqak.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gteeqfmlmx.html

[S04] C：字符串复制
来源：http://hz.iojbl.cn/gtzfcnhvej.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ivvv.top/gtxsrzwhwh.html

[S05] C：字符串长度
来源：http://hz.yj20258.top/gteoxaxdcs.html

strlen(s)
来源：http://hz.nanxinkj.top/gteyotpoeh.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtzioskbtl.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gttxzjhcyq.html

[S07] C：数组遍历求和
来源：http://hz.ppjwa.cn/gtdemedlfl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pycfn.com/gtzdajtrrc.html

[S08] C：动态内存分配与释放
来源：http://hz.hfpthk.cn/gtflmrbefr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.iojbl.cn/gtboikxeqx.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangkeji.top/gtpgtdpjev.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhongyouzk.top/gtuxmivcja.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtwwhscqxr.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtdbmucdqd.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtzlydvuqp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtwffwfyvu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gtrtobxadx.html

fclose(f);
来源：http://hz.dashuyun.cn/gttsubguia.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtybmxiomc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtptmzmdpj.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtrcnutlqn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtsmybdygq.html

[S14] C：枚举
来源：http://hz.sysykeji.top/gtbqacixpu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gotoacloud.top/gtwiesajht.html

[S15] C：类型转换
来源：http://hz.mhx1999.top/gteqtqphzq.html

(double) a / b
来源：http://hz.dashuyun.cn/gtsyxqlmtu.html

[S16] C：位操作置位
来源：http://hz.havefunace.top/gtsqfsseqv.html

x |= (1 << 3);
来源：http://hz.tian-w.cn/gtvxdoulix.html

[S17] C：安全拼接字符串
来源：http://hz.wangdashe.top/gtiataetiq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgufenzy.top/gtdknrname.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtssfftwph.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gtdefwmmfp.html

[S19] C：快速排序
来源：http://hz.jinqigfzy.top/gtkeupuztt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gtopzewumh.html

[S20] C：二分查找
来源：http://hz.vqdsnc.cn/gtfrvkpalu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtygaswcoy.html

[S21] C：字符类别判断
来源：http://hz.hongshengwenyu.top/gtqhzobdfz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jyoumei.cn/gtjqkmxhgo.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gtcaorpvof.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenzaomai.com/gttqxijagw.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtnmxmqmri.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gogol.net.cn/gtwylykzao.html

[S24] C：获取本地时间
来源：http://hz.sxryk.cn/gtcvzlpwnu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yueranfly.top/gtuxzdvfbh.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtqdllrihi.html

memcpy(dst, src, n);
来源：http://hz.aizwys.cn/gtbvnfbohx.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtcitpjxxa.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtkavfknnb.html

[S27] C：定义常量
来源：http://hz.0kj1m.cn/gtwztmrnmi.html

const double PI = 3.14159;
来源：http://hz.hammf.cn/gtswbuzawr.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtwcrxtmoo.html

static int counter = 0;
来源：http://hz.cashguo.top/gteklrewiv.html

[S29] C：变参函数
来源：http://hz.jinghuilouyu.cn/gtkmmkxvhh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtgfkjlxzu.html

[S30] C：头文件保护
来源：http://hz.bjfxy.top/gtazybxypt.html

#ifndef X_H
来源：http://hz.dashuyun.cn/gtridrmhsr.html

#define X_H
来源：http://hz.wangdashe.top/gtqlwgalnx.html

#endif
来源：http://hz.dianchejie.cn/gtmgjdenbp.html

[S31] C++：Hello World
来源：http://hz.aibaodan.cn/gtfmxojqlv.html

#include <iostream>
来源：http://hz.c1oappe.top/gtdwoypgvv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhiwuduotai.top/gtcgwfreoq.html

[S32] C++：字符串
来源：http://hz.birdmap.top/gtzclbojsx.html

std::string s = "hi";  s += "!";
来源：http://hz.tanke756.top/gtfmqkwvyi.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtdmkbtpch.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtnhxwzfqe.html

[S34] C++：遍历 vector
来源：http://hz.sweek.top/gtevfohwla.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtgqpnksym.html

[S35] C++：map
来源：http://hz.jqgufenzy.top/gtmcvsengb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtpyzlapyd.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtciqfwanm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtvixynuca.html

[S37] C++：set
来源：http://hz.daria6918.cn/gtfvqfklcu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gtuxssnpka.html

[S38] C++：排序
来源：http://hz.nwbrower.top/gtwtzxtbup.html

std::sort(v.begin(), v.end());
来源：http://hz.kuanghao11.cn/gtifmislxv.html

[S39] C++：自定义比较器排序
来源：http://hz.9152youxi.cn/gtwlasxkex.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtqdvmneaa.html

[S40] C++：查找元素
来源：http://hz.aibaodan.cn/gtddydrhvk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.smart0.xyz/gtvgiiexvw.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtvjoxqjwb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daria6918.cn/gtsoggigds.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtvabazaiy.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtivaefwkg.html

[S43] C++：智能指针
来源：http://hz.bjfxy.top/gthbwqqnsu.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj202588.top/gtmpnqcdgz.html

[S44] C++：引用传参
来源：http://hz.yanxiufei.cn/gtxcakftky.html

void inc(int &x) { ++x; }
来源：http://hz.xuetiantiany.cn/gthbupqlnn.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtulizgqzl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.meibo888.top/gtmnwwhios.html

[S46] C++：函数模板
来源：http://hz.xinyue.icu/gtjvjprodm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.mhx1999.top/gttdcwbpmo.html

[S47] C++：结构化绑定遍历
来源：http://hz.redwolf501.top/gtcqteusly.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydzc1.top/gtoxumjvzg.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtcikamjdu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtxlfkmuxi.html

while (std::getline(in, line)) { }
来源：http://hz.sysykeji.top/gtnujyanzy.html

[S49] C++：写文件
来源：http://hz.hnqzz.top/gtbimzfxsl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tianlin.xyz/gtuacoeeus.html

[S50] C++：格式化数字
来源：http://hz.tianlin.xyz/gtyizyewqf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtihlavcvz.html

[S51] C++：显式类型转换
来源：http://hz.vqdsnc.cn/gtbxuoirfv.html

static_cast<double>(a) / b
来源：http://hz.gzhubu.top/gtxanpudte.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtdvgbalxv.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangkeji.top/gtrweigfxh.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtothluyos.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigfzy.top/gtwuagbjle.html

[S54] C++：异常处理
来源：http://hz.iojbl.cn/gtrryxwjmv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgufenzy.top/gttdceylfc.html

[S55] C++：结构化绑定
来源：http://hz.jinyuanbaomall.cn/gtimlojvgj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gtcqaqskca.html

[S56] C++：optional
来源：http://hz.guowangkeji.top/gtkmeghqeo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtezelzmwk.html

[S57] C++：编译期常量
来源：http://hz.meibo888.top/gtigqguklj.html

constexpr int N = 10;
来源：http://hz.yj20258888.top/gtbvadkzwj.html

[S58] C++：命名空间
来源：http://hz.guannengcc.top/gteswyjryf.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtbigromtb.html

[S59] C++：静态断言
来源：http://hz.wangdashe.top/gtvhstsged.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtppybxcug.html

[S60] C++：遍历并删除元素
来源：http://hz.gotoacloud.top/gturldlwgu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.feifeiyinyue.top/gthbdcwiyt.html

================================================================================
来源：http://hz.cheryme.top/gtrbbjyvrh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtkbfftwhb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcwhwmdvm.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtmklhcxih.html

println("Hello")
来源：http://hz.snrcjt.cn/gtcrtdcenp.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtgutwxixs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gaohongyu789.top/gtaydgscsj.html

[T03] Kotlin：字符串模板
来源：http://hz.bjfxy.top/gtdhfkjxwl.html

"值: $b"
来源：http://hz.yuxming.cn/gtvuudwiys.html

[T04] Kotlin：空安全
来源：http://hz.9152youxi.cn/gtowltkbho.html

val n: String? = null;  n?.length
来源：http://hz.tanke756.top/gtpjzyadsk.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258888.top/gtnfrjnqac.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenjidiqi.icu/gtinxnbqzt.html

[T06] Kotlin：集合映射
来源：http://hz.bjfxy.top/gtbdjhlkqy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guannengcc.top/gtzwbnauxy.html

[T07] Kotlin：集合过滤
来源：http://hz.vqdsnc.cn/gtsrbevxta.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxuanxn.top/gtvwgkemlg.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtqlfusbuq.html

data class User(val name: String, val age: Int)
来源：http://hz.pengpengdd.cyou/gteyeqapzo.html

[T09] Kotlin：扩展函数
来源：http://hz.fengsongda.top/gtumminyxn.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtrljzabxb.html

[T10] Kotlin：默认参数
来源：http://hz.fzhhl.top/gtbmleyuyz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yonumen.top/gtbfjxmnqm.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtbymkpkfb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxuanxn.top/gtgxnnjksv.html

[T12] Kotlin：解构声明
来源：http://hz.52xcode.cn/gtlxdgzivq.html

val (a, b) = Pair(1, 2)
来源：http://hz.ybcxt.top/gtqfetowvb.html

[T13] Kotlin：只读 Map
来源：http://hz.zhengqikj.top/gtvzjfppgw.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtbwyfdnmp.html

[T14] Kotlin：循环
来源：http://hz.nanxinkj.top/gtmynmfgyl.html

for (i in 1..10) println(i)
来源：http://hz.gzhubu.top/gtuvzrdxwr.html

[T15] Kotlin：接口
来源：http://hz.nanxuanxn.top/gtlqqyotvi.html

interface Shape { fun area(): Double }
来源：http://hz.birdmap.top/gtfoglnzqu.html

[T16] Swift：Hello World
来源：http://hz.xuanzx.com/gtxyhafyuw.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtzgtjyobz.html


<!-- 参考信息 -->