代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.birdmap.top/gtwqnxlmvd.html

[R18] 遍历数组
来源：http://hz.bjfxy.top/gtsenyoqrv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dashuyun.cn/gtrfyjffdb.html

[R19] 数组长度
来源：http://hz.jiagoushi.top/gtqbqjkmng.html

echo "${#arr[@]}"
来源：http://hz.sxryk.cn/gtojjfvgde.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtljsakrcx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigufen.top/gtgkclxwhi.html

[R21] 字符串长度
来源：http://hz.shzxlz.cn/gtlbdfitwh.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gttawqyywz.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gtfgzqkfxn.html

echo "${s:0:5}"
来源：http://hz.bjfxy.top/gteyqcqnjs.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtstbavddz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydjk.org.cn/gtforvrlfv.html

[R24] 大小写转换
来源：http://hz.jinqigufen.top/gtegqbikij.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhijiandao.cn/gtarbdmgay.html

[R25] 去后缀 / 去前缀
来源：http://hz.0kj1m.cn/gtkdzcxlfa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xingfuxueyuan.xyz/gtgqnjykjq.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtnhwmyhkq.html

now=$(date +%F); echo "$now"
来源：http://hz.shangyingyoupin.top/gtllzugfts.html

[R27] 算术展开
来源：http://hz.sufxvd.cn/gtfkmlusts.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtovtihrrt.html

[R28] 浮点运算
来源：http://hz.chenjidiqi.icu/gtqnvdtpdd.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtwexgkixm.html

[R29] 定义函数
来源：http://hz.jlsjyb.cn/gtuemmtxpn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhiwuduotai.top/gtfpsgjbgq.html

[R30] 函数返回状态码
来源：http://hz.jiagoushi.top/gtloxguwko.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.smart0.xyz/gthqbakvvi.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtadpherkt.html

f() { local x=1; echo "$x"; }
来源：http://hz.dianchejie.cn/gtqgzmqqdc.html

[R32] 参数个数校验
来源：http://hz.shangyingyoupin.top/gtadriumpp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtsdjgrdoa.html

[R33] 捕获错误并提示行号
来源：http://hz.feifeiyinyue.top/gtjkbolqih.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtvvgwgazy.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gteltulhqx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtuhtnqvdk.html

[R35] 后台执行并等待
来源：http://hz.0kj1m.cn/gtlfprcwmx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.vqdsnc.cn/gtqclctcwj.html

[R36] 并发执行多个任务
来源：http://hz.gaohongyu789.top/gtepknzfdk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtalvwhato.html

[R37] 把输出赋给变量
来源：http://hz.pengpengdd.cyou/gtljmktysl.html

files=$(ls -1)
来源：http://hz.xylfe.cn/gtrrreaupz.html

[R38] 管道串联
来源：http://hz.tanke756.top/gtywucktvf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtgoplqvke.html

[R39] 重定向标准输出与错误
来源：http://hz.ydzc1.top/gtaithqtvv.html

cmd > out.log 2>&1
来源：http://hz.jyoumei.cn/gtcrlhzags.html

[R40] 追加写日志
来源：http://hz.aizwys.cn/gtrkgtfuqd.html

echo "log" >> out.log
来源：http://hz.xuanzx.com/gtvqouldmc.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtdqkcople.html

cmd >/dev/null 2>&1
来源：http://hz.xziqi.cn/gttdbbmfbm.html

[R42] 输入重定向
来源：http://hz.yj20258.top/gtxultrvht.html

wc -l < a.txt
来源：http://hz.yj20258888.top/gtexwglhxd.html

[R43] 按名字查找文件
来源：http://hz.meibo888.top/gtylscpiau.html

find . -name "*.log" -type f
来源：http://hz.xuetiantiany.cn/gtsnchgenm.html

[R44] 按修改时间查找
来源：http://hz.shangyingyoupin.top/gtmznrqpin.html

find . -mtime -7 -type f
来源：http://hz.daxiang520.top/gtcvfjhcld.html

[R45] 批量删除
来源：http://hz.yueranfly.top/gtgtgtklrb.html

find . -name "*.tmp" -delete
来源：http://hz.ehwqpu.com/gtynbrfwwx.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gttntfdgeq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtacqjkjhp.html

[R47] sed 单行替换
来源：http://hz.fengsongda.top/gtscjzzmth.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenzaomai.com/gtbliyfgff.html

[R48] awk 取指定列
来源：http://hz.ivvv.top/gtjyjnmngl.html

awk '{print $1, $3}' a.txt
来源：http://hz.bjfxy.top/gtkykievus.html

[R49] awk 带条件
来源：http://hz.gaohongyu789.top/gtvhgrlppz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtwstfeqln.html

[R50] awk 求和
来源：http://hz.sweek.top/gtqqqekyos.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangdashe.top/gtkdhnldrn.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtzqpztlhs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtpgxtyiai.html

[R52] 统计行数
来源：http://hz.mhx1999.top/gtpxjthzuf.html

wc -l a.txt
来源：http://hz.pengpengdd.cyou/gtjyvhomsp.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtqyqbbmab.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtathyunvj.html

[R54] 比较两个文件
来源：http://hz.zycfv.cn/gtcwoazhek.html

diff a.txt b.txt
来源：http://hz.hammf.cn/gtmzxaoxph.html

[R55] 压缩与解压
来源：http://hz.0kj1m.cn/gtutvyjiij.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shangyingyoupin.top/gtbryshqcv.html

[R56] 远程拷贝
来源：http://hz.shangyingyoupin.top/gtismrgdrt.html

scp file user@host:/path/
来源：http://hz.hnqzz.top/gtcqddnhea.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtxlkwwgri.html

ssh user@host 'uptime'
来源：http://hz.hnxiangtu.top/gttyxpehjb.html

[R58] 下载文件
来源：http://hz.birdmap.top/gteobwmgka.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xylfe.cn/gtlqqepqfm.html

[R59] 发 POST JSON
来源：http://hz.birdmap.top/gtjlesbwea.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gtsswjonde.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtfewjgvbh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aizwys.cn/gtycmyrkqh.html

[R61] 磁盘占用
来源：http://hz.hysaishi.cn/gtrmhxpmvj.html

df -h;  du -sh *
来源：http://hz.aizwys.cn/gtshdsznlh.html

[R62] 找最占空间的文件
来源：http://hz.sysykeji.top/gtsubziomx.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtybrxafzi.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtoyybxzmf.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gtqnysodjm.html

[R64] 结束进程
来源：http://hz.316326.xyz/gtelukrijk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtnszjjxqo.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtterpnimx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj202588.top/gtvymwjdfp.html

[R66] 定时任务
来源：http://hz.tanke756.top/gtmsoboeos.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtahemnhom.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtfxuxjjja.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtybusrofo.html

[R68] 计算文件校验值
来源：http://hz.jqgfzy.top/gtbtxkcqew.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.vqdsnc.cn/gteqbcdkqh.html

[R69] 生成随机密码
来源：http://hz.hfpthk.cn/gtevecczvc.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtwbgpqeoy.html

[R70] 时间戳与互转
来源：http://hz.mhx1999.top/gtlumswzey.html

date +%s;  date -d @1700000000
来源：http://hz.cheryme.top/gtgmbbmffx.html

[R71] 日期格式化
来源：http://hz.chenlongwang.top/gtilktlbno.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtmefaeras.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtaaiolxaa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gteuyvytgv.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gtsefsmrjn.html

split -l 1000 big.log part_
来源：http://hz.xziqi.cn/gtojgblmve.html

[R74] 批量重命名
来源：http://hz.zhongyouzk.top/gtdzelxcfo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtjrpamgwr.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtrrhbeicl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtckxiexql.html

[R76] 使用临时文件
来源：http://hz.feifeiyinyue.top/gtzgznpnmy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtevlezdwc.html

[R77] 读取用户输入
来源：http://hz.vqdsnc.cn/gtwcwptssd.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gteghfvezn.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtqtfstylz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cqqwz.cn/gtupftmoes.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtfokmjnyk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.svipenyu.cn/gtkhsdyyya.html

[R80] 查看脚本执行耗时
来源：http://hz.jiagoushi.top/gtuqlcorgu.html

time ./run.sh
来源：http://hz.gzhubu.top/gttnmdgviv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfingqukp.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtizpxhquc.html

================================================================================
来源：http://hz.jiagoushi.top/gtpefmgrcs.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtlyjztoqq.html

#include <stdio.h>
来源：http://hz.bjfxy.top/gtwundtbkc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhixingplan.top/gtuklxzyft.html

[S02] C：变量与格式化输出
来源：http://hz.bjfxy.top/gticitbytb.html

int a = 10; printf("%d\n", a);
来源：http://hz.c1oappe.top/gtgiesmvhh.html

[S03] C：读入整数
来源：http://hz.guannengcc.top/gtrhuiabnt.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gttbnzgtae.html

[S04] C：字符串复制
来源：http://hz.shuidangran.top/gtilltympx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuanzhike.top/gtoqeuxenf.html

[S05] C：字符串长度
来源：http://hz.zhixingplan.top/gtlmadjule.html

strlen(s)
来源：http://hz.kuanghao11.cn/gtwyfbuzeo.html

[S06] C：字符串比较
来源：http://hz.zhoulong.xyz/gtdhvjyrdi.html

strcmp(a, b) == 0
来源：http://hz.hywenlv.cn/gtgwnncddn.html

[S07] C：数组遍历求和
来源：http://hz.chenjidiqi.icu/gtozripefm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.snrcjt.cn/gtzrywtxge.html

[S08] C：动态内存分配与释放
来源：http://hz.yvedp.cn/gtzyvtanhf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhongyouzk.top/gtljuzcvwg.html

[S09] C：结构体定义与初始化
来源：http://hz.yuxming.cn/gtthunzugv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenzaomai.com/gteolsbuqd.html

[S10] C：指针与解引用
来源：http://hz.jinqigfzy.top/gtqspkpsrv.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigfzy.top/gtewfgkzyt.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtupmcpmzc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dashuyun.cn/gtskcesgrp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtnhxcynjf.html

fclose(f);
来源：http://hz.zhoulong.xyz/gtpfgugmbf.html

[S12] C：写文件
来源：http://hz.gzhubu.top/gtfimdpwvv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtbgrfozkp.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtrwhjgybw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gtvebnycva.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtytdwwsrq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinyuanbaomall.cn/gtrkynwfzy.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gttpmfcnge.html

(double) a / b
来源：http://hz.shanyushiyangtech.top/gtkktdikpw.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gtkfkbepzv.html

x |= (1 << 3);
来源：http://hz.yj20258888.top/gtexkhgafb.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtfxxfjofj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gttyzgvuyl.html

[S18] C：命令行参数
来源：http://hz.hywenlv.cn/gtnkowreyl.html

int main(int argc, char **argv)
来源：http://hz.yuxming.cn/gtahpnqpxh.html

[S19] C：快速排序
来源：http://hz.zycfv.cn/gtnnntwwfu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xylfe.cn/gtxvsnbgel.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtawsqsjqa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtkxgbxfqr.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gtztaomoyv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cdnleiting.top/gtofbmsydq.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtlugsizgs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gtzsjwgthb.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtkjxtrjgy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jianghu66.top/gtqfdbcfnt.html

[S24] C：获取本地时间
来源：http://hz.52xcode.cn/gtckwdhbvy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtzuxtdkhx.html

[S25] C：内存拷贝
来源：http://hz.ywan-chungtsiang.top/gtwvmlline.html

memcpy(dst, src, n);
来源：http://hz.nanxinkj.top/gtqzimieet.html

[S26] C：内存清零
来源：http://hz.quarkkingdee.top/gtpisjgnbd.html

memset(a, 0, sizeof a);
来源：http://hz.yvedp.cn/gtuixrfzug.html

[S27] C：定义常量
来源：http://hz.svipenyu.cn/gtvcgnnwdr.html

const double PI = 3.14159;
来源：http://hz.dashuyun.cn/gtwicfwvcc.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtwedbakzs.html

static int counter = 0;
来源：http://hz.nanxinkj.top/gtalazhbbt.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtiemrzmem.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtdxhmccwl.html

[S30] C：头文件保护
来源：http://hz.sufxvd.cn/gtwjmdhsdc.html

#ifndef X_H
来源：http://hz.jiagoushi.top/gtobyhdtjx.html

#define X_H
来源：http://hz.zhixingplan.top/gtmvfmnhxt.html

#endif
来源：http://hz.sxryk.cn/gtlikncbnn.html

[S31] C++：Hello World
来源：http://hz.zhongyouzk.top/gtqojkcbpj.html

#include <iostream>
来源：http://hz.wangdashe.top/gttwjjiqib.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jiagoushi.top/gtsoejxmqs.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtdcygfxgg.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gtrsarbucp.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtbzyyilod.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangtech.top/gtpjkfodur.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtyzpfbyih.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yonumen.top/gtuhqybocp.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtglhkhqvq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daria6918.cn/gthpihiuqq.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtlbtufkld.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtybbkobla.html

[S37] C++：set
来源：http://hz.xingfuxueyuan.xyz/gtwrmhraqu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.svipenyu.cn/gtwpguscrs.html

[S38] C++：排序
来源：http://hz.svipenyu.cn/gtbzthgcfd.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtnezraiqc.html

[S39] C++：自定义比较器排序
来源：http://hz.quarkkingdee.top/gtugwvrjuc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.vqdsnc.cn/gtwjgnyxqr.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangkeji.top/gtghalkjcs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnxiangtu.top/gtiolmdvqc.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gtujzkiydt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtrpawevso.html

[S42] C++：继承与虚函数
来源：http://hz.ppjwa.cn/gtcdrcdqiq.html

class B : public Base { public: void f() override {} };
来源：http://hz.gzhubu.top/gtexryhkze.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtaojnphaj.html

auto p = std::make_unique<int>(5);
来源：http://hz.jiagoushi.top/gtnkwzeirg.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtucladlsz.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtxxwkpzsx.html

[S45] C++：lambda
来源：http://hz.iojbl.cn/gtvcjvxxwg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gttroeiavu.html

[S46] C++：函数模板
来源：http://hz.havefunace.top/gtjjdhjzpp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shzxlz.cn/gtsuzkyyjn.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gtecxgwvtm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangkeji.top/gtmmvmdfvx.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtpwlmtxiq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtfhykrnpn.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gtnvefnbdf.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gtysckhclx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtxavpakvq.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtwtwufwvr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gtcwbxriyc.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtcczvuuqe.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gtmjetqqcv.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtciskrshq.html

int size() const noexcept { return n_; }
来源：http://hz.jianghu66.top/gtbdibdcuw.html

[S53] C++：移动语义
来源：http://hz.svipenyu.cn/gtxzajdfsg.html

std::vector<int> w = std::move(v);
来源：http://hz.bjfxy.top/gtemjdefxo.html

[S54] C++：异常处理
来源：http://hz.ybcxt.top/gtkmupeapc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtoxkuusto.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtnlqderbc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtrpbgwnpq.html

[S56] C++：optional
来源：http://hz.jinghuilouyu.cn/gtnazbkwiw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj202588.top/gtqukyvqxu.html

[S57] C++：编译期常量
来源：http://hz.zycfv.cn/gtokucrbev.html

constexpr int N = 10;
来源：http://hz.pengpengdd.cyou/gtzblflggy.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtsraqwzgz.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigufen.top/gticcvyjjj.html

[S59] C++：静态断言
来源：http://hz.yonumen.top/gtihqpvbhe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangshuangyany.cn/gtorjeetyu.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtbpcppgzv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenzaomai.com/gtbotmseqi.html

================================================================================
来源：http://hz.c1oappe.top/gtnaxjhxtn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtrksamfiv.html

================================================================================
来源：http://hz.yvedp.cn/gtbonlwzzn.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gttxlmlcex.html

println("Hello")
来源：http://hz.xziqi.cn/gtwbcwfenx.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gtahggufbw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtxrzxzxqk.html

[T03] Kotlin：字符串模板
来源：http://hz.yonumen.top/gtkwivmufw.html

"值: $b"
来源：http://hz.hammf.cn/gtihfmcalp.html

[T04] Kotlin：空安全
来源：http://hz.chenjidiqi.icu/gtnucvccsp.html

val n: String? = null;  n?.length
来源：http://hz.yanxiufei.cn/gtzbousykp.html

[T05] Kotlin：when 表达式
来源：http://hz.yuanzhike.top/gtrkvuthws.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinyuanbaomall.cn/gtfktyoljs.html

[T06] Kotlin：集合映射
来源：http://hz.bjfxy.top/gttbxrnwyc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuanzx.com/gtvnyhbxjn.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtcmaqhynw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aibaodan.cn/gtmofktbda.html

[T08] Kotlin：数据类
来源：http://hz.zhengqikj.top/gtbgdpoudu.html

data class User(val name: String, val age: Int)
来源：http://hz.svipenyu.cn/gtiqkyznbi.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtbivugzga.html

fun String.exclaim() = this + "!"
来源：http://hz.pycfn.com/gtcjltbqsl.html

[T10] Kotlin：默认参数
来源：http://hz.gotoacloud.top/gtmqzgqvvd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jyoumei.cn/gtiinavrtn.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtpnyfuxoq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gtqingzcki.html

[T12] Kotlin：解构声明
来源：http://hz.0kj1m.cn/gthrgeifii.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtggzfrwnd.html

[T13] Kotlin：只读 Map
来源：http://hz.hnqzz.top/gtuftngbkv.html

val m = mapOf("a" to 1)
来源：http://hz.fzhhl.top/gttwigejtq.html

[T14] Kotlin：循环
来源：http://hz.316326.xyz/gtoowkjlxd.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtqncoqchi.html

[T15] Kotlin：接口
来源：http://hz.jqgufenzy.top/gtmigsocvq.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtgwqzonlc.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtufvtqxdl.html

print("Hello")
来源：http://hz.guannengcc.top/gtgsvvsxbh.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtylsvmjyn.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtqjsghhdj.html

[T18] Swift：字符串插值
来源：http://hz.gotoacloud.top/gtryrefihp.html

"值: \(b)"
来源：http://hz.jianghu66.top/gtdmfctvqv.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangtech.top/gtlajdnbiq.html

if let n = opt { print(n) }
来源：http://hz.haohaochexian.top/gtkzicssoq.html

[T20] Swift：数组操作
来源：http://hz.xylfe.cn/gtpjtlseym.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtqlfcpope.html


<!-- 参考信息 -->