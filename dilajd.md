代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.guannengcc.top/gtzfmfwbxp.html

[R14] C 风格 for
来源：http://hz.aibaodan.cn/gtzniqwgof.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtjlgoazhr.html

[R15] while 逐行读文件
来源：http://hz.hongshengwenyu.top/gtdgsoskas.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtopqimbjy.html

[R16] until 等待条件
来源：http://hz.havefunace.top/gtfvlptthw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gttanozstp.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtaukmtslx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zdqjudy.top/gtofddciwi.html

[R18] 遍历数组
来源：http://hz.hongshengwenyu.top/gtjjbnrali.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnxiangtu.top/gtmbjkkclx.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtmjhypwel.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtzngywnsr.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtjkcabrvb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zycfv.cn/gturrcpeei.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtttqqsbld.html

echo "${#s}"
来源：http://hz.daria6918.cn/gtiedpftcf.html

[R22] 截取子串
来源：http://hz.gotoacloud.top/gtyscoryaa.html

echo "${s:0:5}"
来源：http://hz.sweek.top/gtjjgbbmmc.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gtunwkwkrv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jlsjyb.cn/gtqkqjhsot.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtwiwnjpvd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.svipenyu.cn/gtzdtfnqkj.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtxznfjamq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gttrxozjms.html

[R26] 命令替换
来源：http://hz.nanxuanxn.top/gtiihxprqh.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtziwnsvco.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtlapapwgt.html

echo $((1 + 2 * 3))
来源：http://hz.shuidangran.top/gthgzxdveq.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtdzjdzbql.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgfzy.top/gtxdireuuo.html

[R29] 定义函数
来源：http://hz.xinyue.icu/gtsnvizxkn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtjnrjhoyp.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtazivsdsq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shzxlz.cn/gtkdhaolxe.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtdhjujcyi.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtpwgzijqb.html

[R32] 参数个数校验
来源：http://hz.jinghuilouyu.cn/gtrwwxfhru.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtsgexhxjy.html

[R33] 捕获错误并提示行号
来源：http://hz.smart0.xyz/gtqpmocxrh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yueranfly.top/gtbtehpevl.html

[R34] 退出时清理
来源：http://hz.316326.xyz/gtysqyekge.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gthpanflac.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtkcekzpht.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtbjrqodkm.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtiglvhzos.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gtalwrsbsq.html

[R37] 把输出赋给变量
来源：http://hz.snrcjt.cn/gtgaqibjju.html

files=$(ls -1)
来源：http://hz.shuidangran.top/gtkrobrdln.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtpcfzezes.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtluowksam.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtzlojrngs.html

cmd > out.log 2>&1
来源：http://hz.yvedp.cn/gtffskcppd.html

[R40] 追加写日志
来源：http://hz.jinyuanbaomall.cn/gtarijxzst.html

echo "log" >> out.log
来源：http://hz.jinqigufen.top/gtcivlbahn.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtfzhttxec.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gteynotxru.html

[R42] 输入重定向
来源：http://hz.ivvv.top/gtxfwwrvwm.html

wc -l < a.txt
来源：http://hz.ivvv.top/gtxnccodgd.html

[R43] 按名字查找文件
来源：http://hz.sufxvd.cn/gtonvqptjr.html

find . -name "*.log" -type f
来源：http://hz.c1oappe.top/gtiexvbtks.html

[R44] 按修改时间查找
来源：http://hz.9152youxi.cn/gtrseppnhc.html

find . -mtime -7 -type f
来源：http://hz.cucudq.cn/gtwyjbltis.html

[R45] 批量删除
来源：http://hz.snrcjt.cn/gtpquivexo.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtgaseoeyq.html

[R46] 递归替换文件内容
来源：http://hz.fzhhl.top/gtzjwhoqud.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shangyingyoupin.top/gtvoxcjkah.html

[R47] sed 单行替换
来源：http://hz.feifeiyinyue.top/gtsrzkuguq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangtech.top/gtiobybltn.html

[R48] awk 取指定列
来源：http://hz.ehwqpu.com/gtnhwcanda.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhiwuduotai.top/gtsflnjciq.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtdyclukgr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xylfe.cn/gtjhtoympu.html

[R50] awk 求和
来源：http://hz.yvedp.cn/gtqtgvdvcw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgfzy.top/gterdimahi.html

[R51] 排序去重取前几
来源：http://hz.zhijiandao.cn/gtpwxjubjc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.iojbl.cn/gteulqpobp.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gtodzsflek.html

wc -l a.txt
来源：http://hz.zhoulong.xyz/gtefspzmvp.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtwoxwrgyl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cashguo.top/gtfrjohusu.html

[R54] 比较两个文件
来源：http://hz.chenzaomai.com/gtrpqchwfx.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtserazzyv.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtcbdxhkwn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gthtzzfpzf.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtmrqzxzwl.html

scp file user@host:/path/
来源：http://hz.xuetiantiany.cn/gthgwyxgsm.html

[R57] 远程执行命令
来源：http://hz.chenzaomai.com/gtbdqgjtux.html

ssh user@host 'uptime'
来源：http://hz.xuanzx.com/gtclahotsl.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtvqozdeoj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtwxvztmyl.html

[R59] 发 POST JSON
来源：http://hz.nanxuanxn.top/gtrpzreaxz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtjzykirha.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gtkxnbwhgi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtulbzxfgh.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtivarqvxc.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gtpxoskbkr.html

[R62] 找最占空间的文件
来源：http://hz.snrcjt.cn/gtfnuethrd.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtvkelqrut.html

[R63] 内存与进程
来源：http://hz.zhoulong.xyz/gtqnqwfite.html

free -h;  ps aux | grep nginx
来源：http://hz.52xcode.cn/gtizttmksf.html

[R64] 结束进程
来源：http://hz.chenzaomai.com/gtqoaunctp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtpmsrfaty.html

[R65] 查看端口占用
来源：http://hz.zycfv.cn/gthdndsoip.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.snrcjt.cn/gtoiuxzunu.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gthhjkllmq.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtpljrthvl.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtkcqkgxiq.html

openssl rand -hex 16
来源：http://hz.chenlongwang.top/gtywisqdxt.html

[R68] 计算文件校验值
来源：http://hz.guannengcc.top/gtzjjjnhec.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtrykhkpks.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtwqxvvzvf.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnqzz.top/gtnwstsswv.html

[R70] 时间戳与互转
来源：http://hz.gotoacloud.top/gtekgurcvv.html

date +%s;  date -d @1700000000
来源：http://hz.sxryk.cn/gtnwgzsjuh.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtrfxntgqk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtuabfjrkd.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtjkguncmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sysykeji.top/gttbvbzwtg.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtekojawar.html

split -l 1000 big.log part_
来源：http://hz.pycfn.com/gtlrccvzzi.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gtjslnyfgc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jianghu66.top/gtmdodanfb.html

[R75] 导出环境变量
来源：http://hz.shzxlz.cn/gtnbblypbl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.havefunace.top/gtopbwgrjz.html

[R76] 使用临时文件
来源：http://hz.yanxiufei.cn/gtaafdlkri.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtnwitlink.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtlxevbojy.html

read -rp "请输入: " ans
来源：http://hz.zhixingplan.top/gtnayuuexl.html

[R78] 交互式菜单
来源：http://hz.jqgfzy.top/gtxnayezaa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258888.top/gtsigvycoj.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtwzznuqrb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhixingplan.top/gtoazxpuzx.html

[R80] 查看脚本执行耗时
来源：http://hz.vqdsnc.cn/gtggepctbb.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gttrpuqjtl.html

================================================================================
来源：http://hz.ehwqpu.com/gtunlhznwx.html

S. C / C++ 专题
来源：http://hz.nwbrower.top/gtadjhqmrz.html

================================================================================
来源：http://hz.c1oappe.top/gtxgrvkete.html

[S01] C：Hello World
来源：http://hz.nanxuanxn.top/gtdmdrrkzq.html

#include <stdio.h>
来源：http://hz.tianlin.xyz/gtfzuxvwub.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtjgkmpntr.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtdkmwfxro.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gturynvyad.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtspybjkbu.html

int x; scanf("%d", &x);
来源：http://hz.shzxlz.cn/gtvweanzvm.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtwltjqpad.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gtizarihwa.html

[S05] C：字符串长度
来源：http://hz.316326.xyz/gtwxlhiaph.html

strlen(s)
来源：http://hz.9152youxi.cn/gtscggoock.html

[S06] C：字符串比较
来源：http://hz.pycfn.com/gtybkoeklk.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtdefgrigi.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtdzpnhpll.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zdqjudy.top/gtrrxfkvax.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtqptvjmnk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtlzhxonke.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtvzsvvppf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.redwolf501.top/gtjkdtpqyx.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtgsntrirh.html

int *p = &a;  *p = 5;
来源：http://hz.xuetiantiany.cn/gtybqbamzj.html

[S11] C：逐行读文件
来源：http://hz.cashguo.top/gtebellyiq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtqumnquvs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hongshengwenyu.top/gtcumuemxl.html

fclose(f);
来源：http://hz.hnxiangtu.top/gtntdlnvoq.html

[S12] C：写文件
来源：http://hz.jinqigufen.top/gtoynishji.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gtrbstsuer.html

[S13] C：宏定义
来源：http://hz.zdqjudy.top/gtvkuunlqb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtcktxwvqi.html

[S14] C：枚举
来源：http://hz.gaohongyu789.top/gtorayzxhu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtobnbwbdn.html

[S15] C：类型转换
来源：http://hz.feifeiyinyue.top/gtvyalexdh.html

(double) a / b
来源：http://hz.hfpthk.cn/gtjoruoqcq.html

[S16] C：位操作置位
来源：http://hz.jinqigfzy.top/gtmrzvaxpw.html

x |= (1 << 3);
来源：http://hz.yj20258888.top/gtsodkalko.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtlgrarxrc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.smart0.xyz/gtamabhyqg.html

[S18] C：命令行参数
来源：http://hz.redwolf501.top/gtttiytyab.html

int main(int argc, char **argv)
来源：http://hz.vqdsnc.cn/gtxnsrircs.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gtpnebjbzw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtaqydauya.html

[S20] C：二分查找
来源：http://hz.aibaodan.cn/gtjbzazumq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtexeusmbq.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtgsfslfoa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.iojbl.cn/gtanahwyyv.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gtfoamijyb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.feifeiyinyue.top/gtlogieemy.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtpnkziesd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ppjwa.cn/gtquhosujk.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gtkvspmeni.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtlvdilbti.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gtiawybnwa.html

memcpy(dst, src, n);
来源：http://hz.svipenyu.cn/gtybuuctyj.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtsrhaysvn.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gtymtpuamz.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtlzchnsrm.html

const double PI = 3.14159;
来源：http://hz.daxiang520.top/gtwcqiehxf.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gtoazbpzqp.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gtaaovogkg.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gtvenzqvps.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtbiryvjjr.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtrlarluxl.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtiecwzgbv.html

#define X_H
来源：http://hz.yueranfly.top/gthoboetid.html

#endif
来源：http://hz.meibo888.top/gtjtoraffm.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtevarileo.html

#include <iostream>
来源：http://hz.aibaodan.cn/gtudzpecnp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtmccjzyhj.html

[S32] C++：字符串
来源：http://hz.hammf.cn/gtrmzvcgth.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gthxlmblcf.html

[S33] C++：vector 增删
来源：http://hz.ydzc1.top/gtfyzqjogy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtwnmzzhro.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gthmgakhtj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yongpay.top/gtonoaegbn.html

[S35] C++：map
来源：http://hz.yuanzhike.top/gtmkivvlyg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gthfmznjgt.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gtkqwkgvln.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtsrhabrrc.html

[S37] C++：set
来源：http://hz.yuxming.cn/gtztmafpys.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zycfv.cn/gttrcdkmxd.html

[S38] C++：排序
来源：http://hz.hnxiangtu.top/gtqzyyjxtp.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtraqplyxr.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtnqqwtwcr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.feifeiyinyue.top/gtzdwytxyu.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gtvoudrnwh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtwqdtbemn.html

[S41] C++：类与构造函数
来源：http://hz.daria6918.cn/gtwgfauqxn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hammf.cn/gtlzuvvzkh.html

[S42] C++：继承与虚函数
来源：http://hz.feifeiyinyue.top/gtlsevhcgu.html

class B : public Base { public: void f() override {} };
来源：http://hz.mhx1999.top/gtftabqvrd.html

[S43] C++：智能指针
来源：http://hz.c1oappe.top/gtctidblig.html

auto p = std::make_unique<int>(5);
来源：http://hz.hongshengwenyu.top/gthpimjfin.html

[S44] C++：引用传参
来源：http://hz.andypj.xyz/gtqkghbrmx.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtxfjvvhmh.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtssfhlctt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.0kj1m.cn/gtxjhflkoq.html

[S46] C++：函数模板
来源：http://hz.yj20258888.top/gtmycdplsp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.birdmap.top/gtwpbgdbij.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gttwsrnbkz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtuagjxurv.html

[S48] C++：逐行读文件
来源：http://hz.jqgfzy.top/gtrhcrqnnb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtwhihdvzp.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtlujhzpgo.html

[S49] C++：写文件
来源：http://hz.shanyushiyangtech.top/gtfvafldrt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yangfankeji.com/gtjpsrwkgz.html

[S50] C++：格式化数字
来源：http://hz.hammf.cn/gtsvzaqhgd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnxiangtu.top/gtbpkprfmy.html

[S51] C++：显式类型转换
来源：http://hz.zycfv.cn/gtjodzbpbv.html

static_cast<double>(a) / b
来源：http://hz.gogol.net.cn/gtmicodxwx.html

[S52] C++：const 与 noexcept
来源：http://hz.sufxvd.cn/gtvpgzyrnl.html

int size() const noexcept { return n_; }
来源：http://hz.zhiwuduotai.top/gtqrykwgte.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gthptewszl.html

std::vector<int> w = std::move(v);
来源：http://hz.xingfuxueyuan.xyz/gtbtsyrwnf.html

[S54] C++：异常处理
来源：http://hz.yj202588.top/gtqcjbiohh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtywsoqcah.html

[S55] C++：结构化绑定
来源：http://hz.meibo888.top/gtdgjwzowq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yvedp.cn/gtsmytovnl.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtzhkegrpm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenjidiqi.icu/gtlwwzcdfh.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gtvmssnlez.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gtvjyucjld.html

[S58] C++：命名空间
来源：http://hz.0kj1m.cn/gtivvvvxty.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtnpidcuje.html

[S59] C++：静态断言
来源：http://hz.yj202588.top/gtskmdjjvr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xingfuxueyuan.xyz/gtthagdmnx.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtteizxvak.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj202588.top/gtgazvxipo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvivkiizg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aibaodan.cn/gtxyljegli.html

================================================================================
来源：http://hz.52xcode.cn/gtiezheizd.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gthoqwsndd.html

println("Hello")
来源：http://hz.havefunace.top/gtyidqeevy.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtaajtnbye.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenjidiqi.icu/gtrihzhwjd.html

[T03] Kotlin：字符串模板
来源：http://hz.mhx1999.top/gtqomliibz.html

"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtxlgvjcxb.html

[T04] Kotlin：空安全
来源：http://hz.dianchejie.cn/gtvfxkuyyk.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtitdhnwys.html

[T05] Kotlin：when 表达式
来源：http://hz.hfpthk.cn/gtmmqditcd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zdqjudy.top/gtaoalxaub.html

[T06] Kotlin：集合映射
来源：http://hz.bjfxy.top/gtyvagfkaf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.haohaochexian.top/gtenufpuls.html

[T07] Kotlin：集合过滤
来源：http://hz.hnxiangtu.top/gtuycapgjc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.havefunace.top/gtxbzrxyiv.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtpcucklbu.html

data class User(val name: String, val age: Int)
来源：http://hz.pycfn.com/gtttbnhnsq.html

[T09] Kotlin：扩展函数
来源：http://hz.birdmap.top/gtcdleajkl.html

fun String.exclaim() = this + "!"
来源：http://hz.zycfv.cn/gtpxjyndnl.html

[T10] Kotlin：默认参数
来源：http://hz.yvedp.cn/gttwbrdavt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtpkcbwciy.html

[T11] Kotlin：协程
来源：http://hz.feifeiyinyue.top/gtwnphdcfa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cqqwz.cn/gtevrsbnyx.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtacmtlojp.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtxivnxdkg.html

[T13] Kotlin：只读 Map
来源：http://hz.gaohongyu789.top/gtncqmrzef.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtwdtlngfu.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangtech.top/gtfqzxfeub.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gtfwbwoorn.html

[T15] Kotlin：接口
来源：http://hz.yongpay.top/gtkmlpyzvl.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtpmlhvwyf.html

[T16] Swift：Hello World
来源：http://hz.fengsongda.top/gtckouvrfg.html

print("Hello")
来源：http://hz.xylfe.cn/gtoujxnqef.html


<!-- 参考信息 -->