代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangtech.top/gtgfebfpts.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtkulliyyg.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gtmjfopbvk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gotoacloud.top/gtrixhbitp.html

[Q88] 行转列（条件聚合）
来源：http://hz.yangfankeji.com/gttriokgro.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangtech.top/gtplxpabjw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gtpjtfggfr.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gtrfrixhpm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.redwolf501.top/gtdkxoreib.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gttvnqqrut.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtgvtusquq.html

================================================================================
来源：http://hz.guannengcc.top/gtdaogrrcv.html

R. Bash 专题
来源：http://hz.sysykeji.top/gtzhvzdmnn.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvyzxpgmg.html

[R01] shebang 与严格模式
来源：http://hz.cqqwz.cn/gtclipxxag.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtxlwjnfhd.html

set -euo pipefail
来源：http://hz.52xcode.cn/gtuhxknlrn.html

[R02] 变量赋值与使用
来源：http://hz.pycfn.com/gtalkrculs.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gtpervtbmk.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gtbbcujogd.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtgyiuvxtc.html

[R04] 位置参数
来源：http://hz.hfpthk.cn/gtuexjtlxr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.52xcode.cn/gtyokmdhnz.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gthipebdcu.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gtjnxcclpj.html

[R06] 判断命令是否存在
来源：http://hz.cucudq.cn/gtxaqwrtfr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtcuuhrfqz.html

[R07] if 判断文件
来源：http://hz.kuanghao11.cn/gtvyyuddnl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtikraarva.html

[R08] 数值比较
来源：http://hz.jinghuilouyu.cn/gthgairlpm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gtkzlvsgsh.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtqxvtzxlp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtuirewked.html

[R10] 正则匹配
来源：http://hz.ywan-chungtsiang.top/gtmcnypqnu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gtlkkismbu.html

[R11] case 多分支
来源：http://hz.daria6918.cn/gtrifpkvlu.html

case "$1" in
来源：http://hz.cqqwz.cn/gtndyxwkyi.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtuuysnmyb.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtsjcddsvb.html

*)     echo "未知命令" ;;
来源：http://hz.jqgfzy.top/gthlvwgata.html

esac
来源：http://hz.birdmap.top/gtenqgvwlk.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtfjvkqehk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hammf.cn/gturmqsyzn.html

[R13] for 计数循环
来源：http://hz.zhixingplan.top/gtgwwhsqof.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cheryme.top/gttqudqevs.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtyiuadhkl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gtcmlcwzwi.html

[R15] while 逐行读文件
来源：http://hz.gzhubu.top/gtzxfsmylu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtichpghkk.html

[R16] until 等待条件
来源：http://hz.xylfe.cn/gtlfsxeola.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhengqikj.top/gteuqalegk.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtvdmmaojp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhixingplan.top/gtyvdzznhe.html

[R18] 遍历数组
来源：http://hz.aibaodan.cn/gtwnmtihbw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtkcshwnts.html

[R19] 数组长度
来源：http://hz.yj20258888.top/gtgolofmgw.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gtypmdqrnx.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gtlugbkept.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtuctilcao.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtvqtwzglr.html

echo "${#s}"
来源：http://hz.sweek.top/gtqtmcmkra.html

[R22] 截取子串
来源：http://hz.hongshengwenyu.top/gtkijbimjb.html

echo "${s:0:5}"
来源：http://hz.xingfuxueyuan.xyz/gttmsbrnlv.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtgeatafjs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtfidzutiy.html

[R24] 大小写转换
来源：http://hz.pengpengdd.cyou/gtvclhdpgo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtpkcyvljl.html

[R25] 去后缀 / 去前缀
来源：http://hz.cucudq.cn/gtoqrzcuur.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtufxirkkv.html

[R26] 命令替换
来源：http://hz.havefunace.top/gtyevpejaa.html

now=$(date +%F); echo "$now"
来源：http://hz.sxryk.cn/gttdnmnifu.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gteoavjtrp.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtpluyntqi.html

[R28] 浮点运算
来源：http://hz.0kj1m.cn/gtucvstwio.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhongyouzk.top/gtqcphhmtp.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtbeagugwp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtvjujnpgh.html

[R30] 函数返回状态码
来源：http://hz.yj20258.top/gtjbplpkai.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtjhaljbtb.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtendkarho.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtaljleryv.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtcchfssfd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yanxiufei.cn/gtayyhbbax.html

[R33] 捕获错误并提示行号
来源：http://hz.jlsjyb.cn/gtkfydvwbb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtfkmhatcx.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtkddrndkk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.fzhhl.top/gtrzgmvygd.html

[R35] 后台执行并等待
来源：http://hz.yj202588.top/gtmgpkfqze.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ppjwa.cn/gtzaznmsgi.html

[R36] 并发执行多个任务
来源：http://hz.yueranfly.top/gtavrttmaa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.bjfxy.top/gtmntacozp.html

[R37] 把输出赋给变量
来源：http://hz.hongshengwenyu.top/gtluusetnm.html

files=$(ls -1)
来源：http://hz.tianlin.xyz/gtadidehgw.html

[R38] 管道串联
来源：http://hz.yj202588.top/gtdgvfnlsk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtemjvidzv.html

[R39] 重定向标准输出与错误
来源：http://hz.gaohongyu789.top/gtxinbtcfy.html

cmd > out.log 2>&1
来源：http://hz.xuetiantiany.cn/gtsgyncbga.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtvnsngujk.html

echo "log" >> out.log
来源：http://hz.hnqzz.top/gtgfsvibnp.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtqmosmavm.html

cmd >/dev/null 2>&1
来源：http://hz.cashguo.top/gtxydhfjmt.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gtykyeiesg.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtraxoqypm.html

[R43] 按名字查找文件
来源：http://hz.hongshengwenyu.top/gtvigxhynk.html

find . -name "*.log" -type f
来源：http://hz.jqgfzy.top/gtyxqoggov.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtfxgblkuz.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtpykbvpys.html

[R45] 批量删除
来源：http://hz.redwolf501.top/gtkxjzjtvy.html

find . -name "*.tmp" -delete
来源：http://hz.cheryme.top/gtpdxhfvah.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gtbymxwttm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.feifeiyinyue.top/gtajgxfwib.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtjbswutbf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtnmnyxxrv.html

[R48] awk 取指定列
来源：http://hz.svipenyu.cn/gtixkfigoo.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtecrbwceg.html

[R49] awk 带条件
来源：http://hz.sweek.top/gtamccbmkt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgufenzy.top/gtzvhbqhpn.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtrgimwjjj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinghuilouyu.cn/gtgowipsby.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtuixqdnem.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sxryk.cn/gtgggdjosn.html

[R52] 统计行数
来源：http://hz.hammf.cn/gtbuxnshmu.html

wc -l a.txt
来源：http://hz.pengpengdd.cyou/gtaywogeqm.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtajqzugxa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ybcxt.top/gtoxrcgnnr.html

[R54] 比较两个文件
来源：http://hz.cdnleiting.top/gteiwlojrp.html

diff a.txt b.txt
来源：http://hz.gogol.net.cn/gtyenyeihe.html

[R55] 压缩与解压
来源：http://hz.zhixingplan.top/gtqurguhok.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tanke756.top/gtzxbgavip.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtdbpefqns.html

scp file user@host:/path/
来源：http://hz.sweek.top/gterkttiyo.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtpawqlxdr.html

ssh user@host 'uptime'
来源：http://hz.jinqigufen.top/gtipxoedop.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gttgnaaeek.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.bjfxy.top/gtovasqzsy.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtfjcpfndq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.iojbl.cn/gtefiexizj.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtmneafhmt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gthwjwopac.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtfvknfyjq.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtsqrmjcwg.html

[R62] 找最占空间的文件
来源：http://hz.daxiang520.top/gtegulqzzp.html

du -ah . | sort -rh | head -10
来源：http://hz.fzhhl.top/gtbktfsfle.html

[R63] 内存与进程
来源：http://hz.jinqigfzy.top/gtwjcbyvle.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtmxcysdct.html

[R64] 结束进程
来源：http://hz.xinyue.icu/gtwjswitdg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gtuororcdh.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtjqleksma.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gtsvhoaqpf.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtausthcvc.html

crontab -e;  crontab -l
来源：http://hz.dashuyun.cn/gtcmgggwdn.html

[R67] 生成随机十六进制串
来源：http://hz.chenjidiqi.icu/gttuufjkes.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtwdehbcsr.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtqawbpjjr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinyuanbaomall.cn/gtaykvjeqi.html

[R69] 生成随机密码
来源：http://hz.xylfe.cn/gtihmecwht.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtsuvvhsjk.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gtonkiymcu.html

date +%s;  date -d @1700000000
来源：http://hz.jinyuanbaomall.cn/gtwkzwhgvx.html

[R71] 日期格式化
来源：http://hz.havefunace.top/gtyqspqkfn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigfzy.top/gtghahxxyg.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gtxsktusyy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtafnkzsrb.html

[R73] 分割大日志
来源：http://hz.nanxinkj.top/gtannkqjrm.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtmdbvvdph.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtyaoryrhb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gttufmmise.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtfzjbekzn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.snrcjt.cn/gtqmcujavd.html

[R76] 使用临时文件
来源：http://hz.yongpay.top/gtvcmncchw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtlivnkwyd.html

[R77] 读取用户输入
来源：http://hz.jinqigufen.top/gtcpcnsimo.html

read -rp "请输入: " ans
来源：http://hz.0kj1m.cn/gthwiczcxj.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtlvclxiny.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtckplmvwa.html

[R79] 解析命令行选项
来源：http://hz.gzhubu.top/gtuoliysax.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.9152youxi.cn/gtjnbhyyer.html

[R80] 查看脚本执行耗时
来源：http://hz.yuxming.cn/gtpardrzjy.html

time ./run.sh
来源：http://hz.yongpay.top/gtegqapduk.html

================================================================================
来源：http://hz.haohaochexian.top/gtnoimdhsa.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtpnkswidu.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmguputop.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtxatraoif.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtdjpaovpt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gtsydxspgx.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtkpynxwrc.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtohthlmdv.html

[S03] C：读入整数
来源：http://hz.chenlongwang.top/gtwsraqzzz.html

int x; scanf("%d", &x);
来源：http://hz.feifeiyinyue.top/gteotherrd.html

[S04] C：字符串复制
来源：http://hz.iojbl.cn/gtgbkfcgtu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gtbwqyoikm.html

[S05] C：字符串长度
来源：http://hz.jinghuilouyu.cn/gtmxvwmjda.html

strlen(s)
来源：http://hz.hywenlv.cn/gtjpnboior.html

[S06] C：字符串比较
来源：http://hz.zdqjudy.top/gturqwqvzu.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtkgvkoejh.html

[S07] C：数组遍历求和
来源：http://hz.zhiwuduotai.top/gtenxaworm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtnjfkenic.html

[S08] C：动态内存分配与释放
来源：http://hz.jianghu66.top/gtmkxjfyyc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.iojbl.cn/gtaidirlva.html

[S09] C：结构体定义与初始化
来源：http://hz.hnxiangtu.top/gtyoshfuej.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtdecmzzdv.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtdgxljgzi.html

int *p = &a;  *p = 5;
来源：http://hz.quarkkingdee.top/gtdmowdqts.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gthurgnqii.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jyoumei.cn/gtiwgbylvi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cdnleiting.top/gtmqeewmfn.html

fclose(f);
来源：http://hz.fengsongda.top/gtsprmwceo.html

[S12] C：写文件
来源：http://hz.ivvv.top/gtiduxilpb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtmknjazfh.html

[S13] C：宏定义
来源：http://hz.tianlin.xyz/gtyarccxnd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtvchdpswz.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtwlhikkrt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtgxxnrkot.html

[S15] C：类型转换
来源：http://hz.cucudq.cn/gtnxofdzdt.html

(double) a / b
来源：http://hz.zhongyouzk.top/gtjazfacrr.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtdrpasnar.html

x |= (1 << 3);
来源：http://hz.cashguo.top/gtpuymanrl.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258.top/gtnedowobp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtcybwrywz.html

[S18] C：命令行参数
来源：http://hz.hysaishi.cn/gtytbumhfc.html

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gthytmmmhh.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtmveolkhd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtbyuhebrz.html

[S20] C：二分查找
来源：http://hz.cdnleiting.top/gtdyntxbne.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtehiegjim.html

[S21] C：字符类别判断
来源：http://hz.andypj.xyz/gtdvexedzj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtfwsoccek.html

[S22] C：字符串转数字
来源：http://hz.andypj.xyz/gtibosinwa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gttongdinm.html

[S23] C：随机数
来源：http://hz.jiagoushi.top/gtdsmnqfvh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtowxsndqi.html

[S24] C：获取本地时间
来源：http://hz.yueranfly.top/gttagtcuya.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtvexjqiyn.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtrhgogfex.html

memcpy(dst, src, n);
来源：http://hz.jinqigufen.top/gtkqauyekq.html

[S26] C：内存清零
来源：http://hz.cucudq.cn/gtuhimktxu.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtpptueqiz.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gtklrjjfuo.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtskmjxfjs.html

[S28] C：静态变量
来源：http://hz.xylfe.cn/gtoireiaed.html

static int counter = 0;
来源：http://hz.52xcode.cn/gtelfdrgga.html

[S29] C：变参函数
来源：http://hz.shuidangran.top/gttnqabwgn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydzc1.top/gtjrmvvffl.html

[S30] C：头文件保护
来源：http://hz.fengsongda.top/gthbopbkab.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtktxvojmw.html

#define X_H
来源：http://hz.ydjk.org.cn/gtdkuuoxcv.html

#endif
来源：http://hz.hywenlv.cn/gtixrsovhw.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtoyxdjoys.html

#include <iostream>
来源：http://hz.zhongyouzk.top/gtwqwrgmyw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhixingplan.top/gtsutpoarn.html

[S32] C++：字符串
来源：http://hz.chenjidiqi.icu/gtasdkzhpy.html

std::string s = "hi";  s += "!";
来源：http://hz.havefunace.top/gtrwmbildg.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gtboyynawa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtvqulssob.html

[S34] C++：遍历 vector
来源：http://hz.gzhubu.top/gtpfxbhged.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtqqawwhzy.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtajuzmdco.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtpkdwxrlj.html

[S36] C++：unordered_map
来源：http://hz.xuanzx.com/gtovuvdxcq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtblafnfaq.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gthirapgvk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtsllpkftc.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtirbskian.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangtech.top/gtsscyglfp.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigufen.top/gtsvjlvwed.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yvedp.cn/gtolnpesha.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtzwkrbvls.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guannengcc.top/gtpxfwinki.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtwtyzebiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hywenlv.cn/gtfudplucc.html

[S42] C++：继承与虚函数
来源：http://hz.smart0.xyz/gtwvzqjrjf.html

class B : public Base { public: void f() override {} };
来源：http://hz.xylfe.cn/gtsdbzmpjh.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtitdbxzcz.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258888.top/gtqegejknk.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtlkzvvkuf.html

void inc(int &x) { ++x; }
来源：http://hz.xylfe.cn/gtitjlkhog.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtnweghzil.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gtqltdcdgr.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtmvipufxw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtfavoeaxo.html

[S47] C++：结构化绑定遍历
来源：http://hz.cdnleiting.top/gtsnwaintv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtbhjqockt.html

[S48] C++：逐行读文件
来源：http://hz.ydjk.org.cn/gtoreoppaa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtsehnrbuj.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtfvtjvbpo.html

[S49] C++：写文件
来源：http://hz.ppjwa.cn/gtxpzfdjrb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.redwolf501.top/gtxlqafenf.html

[S50] C++：格式化数字
来源：http://hz.jlsjyb.cn/gtjrtbcelf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.bjfxy.top/gtsioxiwjq.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtmlpibdbn.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtrilocdtu.html

[S52] C++：const 与 noexcept
来源：http://hz.bjfxy.top/gtollivewk.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtgqcyvhff.html

[S53] C++：移动语义
来源：http://hz.jiagoushi.top/gtgeztolmx.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gtskcldtvz.html

[S54] C++：异常处理
来源：http://hz.sxryk.cn/gtrissxoog.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtyttzlsdp.html

[S55] C++：结构化绑定
来源：http://hz.wangdashe.top/gtstitxvfg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtaqvjvpfc.html

[S56] C++：optional
来源：http://hz.mhx1999.top/gtblcywhqo.html


<!-- 参考信息 -->