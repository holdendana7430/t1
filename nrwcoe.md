代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.aizwys.cn/gtomyydmqm.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtsxjkcjlm.html

[Q85] 数值取整
来源：http://hz.fengsongda.top/gtkpxzcrvq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gtflkucgjm.html

[Q86] 读取 JSON 字段
来源：http://hz.gaohongyu789.top/gttxhtrrax.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yanxiufei.cn/gtelbsafcy.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtfivzqcck.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuanzx.com/gtcwzsnmfq.html

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtootalgtm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtmsimhkbh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.c1oappe.top/gtgswjzxah.html

[Q89] 判断表是否存在
来源：http://hz.jiagoushi.top/gtnjcgikee.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gtzotvgmth.html

[Q90] 生成序号列
来源：http://hz.jlsjyb.cn/gtqfeptuug.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtidmymiro.html

================================================================================
来源：http://hz.sweek.top/gtowjzmxbk.html

R. Bash 专题
来源：http://hz.birdmap.top/gtgvrogzbz.html

================================================================================
来源：http://hz.sweek.top/gthjeythlw.html

[R01] shebang 与严格模式
来源：http://hz.vqdsnc.cn/gtxpjplaul.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gtsfecoahy.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtnhoehaba.html

[R02] 变量赋值与使用
来源：http://hz.jyoumei.cn/gtdvgoadwm.html

name="Tom"; echo "$name"
来源：http://hz.sufxvd.cn/gtgoieoalc.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gtbmwcczwd.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gtzzvhvwer.html

[R04] 位置参数
来源：http://hz.ehwqpu.com/gtjwwiwgzx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtiillwvxn.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtngppzkow.html

name="${1:-default}"
来源：http://hz.jlsjyb.cn/gtslqwpacf.html

[R06] 判断命令是否存在
来源：http://hz.yvedp.cn/gtcqbjsqun.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydzc1.top/gtuquovftu.html

[R07] if 判断文件
来源：http://hz.gaohongyu789.top/gttqqtoxse.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtrivxafwk.html

[R08] 数值比较
来源：http://hz.ybcxt.top/gtkbzxztnn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gtewrvwiti.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gtbtbrmhrp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.smart0.xyz/gtdznjjjko.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtxwxwlhte.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yanxiufei.cn/gtstlxoixs.html

[R11] case 多分支
来源：http://hz.pycfn.com/gtxeiqbjxr.html

case "$1" in
来源：http://hz.iojbl.cn/gtjmtqbpbd.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtrmuqshss.html

stop)  echo "停止" ;;
来源：http://hz.jinyuanbaomall.cn/gtjkklemgy.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtttanqkdk.html

esac
来源：http://hz.vqdsnc.cn/gtwykkmuvf.html

[R12] for 遍历文件
来源：http://hz.jyoumei.cn/gtawzifzcx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fzhhl.top/gtjcvfvciq.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtpleyxfbk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtlzwdsmdp.html

[R14] C 风格 for
来源：http://hz.smart0.xyz/gttlackmmo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtqhmgqasi.html

[R15] while 逐行读文件
来源：http://hz.yj202588.top/gtgunffwzf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtzynztlel.html

[R16] until 等待条件
来源：http://hz.hywenlv.cn/gtpicmguvo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.redwolf501.top/gtcubnaffe.html

[R17] 数组定义与取值
来源：http://hz.nanxuanxn.top/gtiinhjmvz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtpuvtqewv.html

[R18] 遍历数组
来源：http://hz.chenlongwang.top/gtihvcakkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guowangkeji.top/gtagdivtej.html

[R19] 数组长度
来源：http://hz.hnqzz.top/gtkjyswyyg.html

echo "${#arr[@]}"
来源：http://hz.xziqi.cn/gtcexxovms.html

[R20] 关联数组（字典）
来源：http://hz.andypj.xyz/gtajxbdjcw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtidmnahry.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtsjcjxfrw.html

echo "${#s}"
来源：http://hz.ppjwa.cn/gtibmwcwni.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtgvtufnnq.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gthfcoqnsy.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtjwhacdxc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtepxithzx.html

[R24] 大小写转换
来源：http://hz.yonumen.top/gtbodsvvcz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtvcceunee.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtdmiuntep.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigfzy.top/gtixoforkw.html

[R26] 命令替换
来源：http://hz.jinqigufen.top/gtinpulzeo.html

now=$(date +%F); echo "$now"
来源：http://hz.hysaishi.cn/gttqpnceqb.html

[R27] 算术展开
来源：http://hz.gotoacloud.top/gtitbxludl.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gturpbfxpo.html

[R28] 浮点运算
来源：http://hz.dashuyun.cn/gtypumidpa.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gtwotlotzn.html

[R29] 定义函数
来源：http://hz.zdqjudy.top/gtdxudfgbp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangdashe.top/gtjodkqqqg.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtekmeuwtc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gtxntelhve.html

[R31] 局部变量
来源：http://hz.yj202588.top/gtiwuawpzm.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigfzy.top/gtxmvwinsn.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtddbmwrbm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.haohaochexian.top/gtfzkmxisn.html

[R33] 捕获错误并提示行号
来源：http://hz.vqdsnc.cn/gtxdipsnuh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dianchejie.cn/gtnqhdqdfi.html

[R34] 退出时清理
来源：http://hz.0kj1m.cn/gttddiifzg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.fzhhl.top/gtsutpcusb.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gtrkjtmlij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.0kj1m.cn/gtfxzoprqa.html

[R36] 并发执行多个任务
来源：http://hz.hnqzz.top/gttafqdahx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtaujnqsrm.html

[R37] 把输出赋给变量
来源：http://hz.shzxlz.cn/gtxdboykih.html

files=$(ls -1)
来源：http://hz.ppjwa.cn/gthaaovxak.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtmjeiozhl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtrpsuedqp.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtbtkpfoqe.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtfuwkolqp.html

[R40] 追加写日志
来源：http://hz.zhongyouzk.top/gtljedgenm.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtkzughktp.html

[R41] 丢弃输出
来源：http://hz.yj202588.top/gtkgczirnz.html

cmd >/dev/null 2>&1
来源：http://hz.daria6918.cn/gtniehsnhm.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtomxyhwkw.html

wc -l < a.txt
来源：http://hz.ydzc1.top/gtvlchepav.html

[R43] 按名字查找文件
来源：http://hz.cucudq.cn/gtzoiqxdoq.html

find . -name "*.log" -type f
来源：http://hz.snrcjt.cn/gtdeuipbwj.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtubncffqq.html

find . -mtime -7 -type f
来源：http://hz.ppjwa.cn/gtwraobpep.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtyzkchtvm.html

find . -name "*.tmp" -delete
来源：http://hz.0kj1m.cn/gtzvjtcgbp.html

[R46] 递归替换文件内容
来源：http://hz.redwolf501.top/gtttaezpzn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.0kj1m.cn/gtlssasjsw.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtkmovddnf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhaomingkeji.xyz/gtgxephlze.html

[R48] awk 取指定列
来源：http://hz.guowangkeji.top/gtdfdvnbnf.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtcdtxpkge.html

[R49] awk 带条件
来源：http://hz.gzhubu.top/gtboenrzwv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtiazbqdif.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtgdbdtihv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gaohongyu789.top/gteeslzaih.html

[R51] 排序去重取前几
来源：http://hz.zhixingplan.top/gttkcwqemm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gteorlxwjo.html

[R52] 统计行数
来源：http://hz.hnxiangtu.top/gtzwqzneps.html

wc -l a.txt
来源：http://hz.zhoulong.xyz/gtijofrgvo.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtmjujnmio.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fzhhl.top/gtetdvzvmy.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtmioldqbk.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtdsfyfizc.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtepudpgyv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hongshengwenyu.top/gtyfokgern.html

[R56] 远程拷贝
来源：http://hz.tianlin.xyz/gtqfxjhlpf.html

scp file user@host:/path/
来源：http://hz.yj202588.top/gtqyjkavyj.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtjcvlzksz.html

ssh user@host 'uptime'
来源：http://hz.hnxiangtu.top/gtvronrxiw.html

[R58] 下载文件
来源：http://hz.xziqi.cn/gtgghpifyx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.0kj1m.cn/gtzxvvkrgp.html

[R59] 发 POST JSON
来源：http://hz.xziqi.cn/gtcqijnkdc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cucudq.cn/gtsbwyixsq.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtapxgrxut.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.c1oappe.top/gtonxhlxpe.html

[R61] 磁盘占用
来源：http://hz.andypj.xyz/gtrhzudgnm.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtdjpkxxor.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtkyammsxk.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtsauathht.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gtuspchkra.html

free -h;  ps aux | grep nginx
来源：http://hz.chenjidiqi.icu/gtkwcckgkw.html

[R64] 结束进程
来源：http://hz.vqdsnc.cn/gttvccyqal.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gttemhwunc.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtcpwlljtf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtyefssped.html

[R66] 定时任务
来源：http://hz.shanyushiyangtech.top/gtqkzyllum.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gtmzbvoldg.html

[R67] 生成随机十六进制串
来源：http://hz.gaohongyu789.top/gtyuxhrecm.html

openssl rand -hex 16
来源：http://hz.chenjidiqi.icu/gtautzwmrs.html

[R68] 计算文件校验值
来源：http://hz.jinyuanbaomall.cn/gtzkxajcbl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.316326.xyz/gtmwnvqdof.html

[R69] 生成随机密码
来源：http://hz.ydzc1.top/gtlshfckea.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtmysytyol.html

[R70] 时间戳与互转
来源：http://hz.zhengqikj.top/gtyxexqhky.html

date +%s;  date -d @1700000000
来源：http://hz.xingfuxueyuan.xyz/gtyrigwvlh.html

[R71] 日期格式化
来源：http://hz.ywan-chungtsiang.top/gtdrnwuhjn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuanzhike.top/gtyrvylkab.html

[R72] 等待端口就绪
来源：http://hz.dianchejie.cn/gtqodinoed.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gttmytrbcm.html

[R73] 分割大日志
来源：http://hz.daxiang520.top/gtoyrogxbx.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtqipfsuhm.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtccdjhwdn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuanzx.com/gthbxzhrnv.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtbmgdsdtr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.smart0.xyz/gtccjjwxyh.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtgwxqtfrq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtcltygtfv.html

[R77] 读取用户输入
来源：http://hz.tian-w.cn/gtqkjionkp.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtghgihovk.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtshxmtgek.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtytdkeuvk.html

[R79] 解析命令行选项
来源：http://hz.xingfuxueyuan.xyz/gtbslynnwn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtzycwkvwi.html

[R80] 查看脚本执行耗时
来源：http://hz.xingfuxueyuan.xyz/gtwjvpcnua.html

time ./run.sh
来源：http://hz.chenlongwang.top/gtmdrsswid.html

================================================================================
来源：http://hz.ehwqpu.com/gtkgvqwchy.html

S. C / C++ 专题
来源：http://hz.shangyingyoupin.top/gteecgdzon.html

================================================================================
来源：http://hz.jiagoushi.top/gtukdkjfgr.html

[S01] C：Hello World
来源：http://hz.hywenlv.cn/gtoxapqglk.html

#include <stdio.h>
来源：http://hz.yonumen.top/gtcanhwtky.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cashguo.top/gteelulwir.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gtboowweof.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gtrouzfosy.html

[S03] C：读入整数
来源：http://hz.yangfankeji.com/gtqygtmpsf.html

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtefeieblb.html

[S04] C：字符串复制
来源：http://hz.vqdsnc.cn/gtzsaopkog.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtpnynakrn.html

[S05] C：字符串长度
来源：http://hz.ehwqpu.com/gtejjenpxr.html

strlen(s)
来源：http://hz.ydjk.org.cn/gtnvtmrycs.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtwptlivjx.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtbqjscmre.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtordekhwo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yonumen.top/gtirkqsprd.html

[S08] C：动态内存分配与释放
来源：http://hz.iojbl.cn/gtyugiuvny.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtkrmnfrlk.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gtqqxyaxth.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yanxiufei.cn/gtsjkpwzcx.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtquiqgonm.html

int *p = &a;  *p = 5;
来源：http://hz.kuanghao11.cn/gtwagzyvnb.html

[S11] C：逐行读文件
来源：http://hz.svipenyu.cn/gtfnjbjakr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.snrcjt.cn/gtmuivtmvr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtocbxwiio.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtefpnhnui.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gtssnlbiwc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinghuilouyu.cn/gtdcfeatzb.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtxustcvkw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gaohongyu789.top/gttqkhsguv.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtqkaqlebv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhijiandao.cn/gtumqaxbjl.html

[S15] C：类型转换
来源：http://hz.guowangkeji.top/gtmgclgcdh.html

(double) a / b
来源：http://hz.ivvv.top/gtjedcugdl.html

[S16] C：位操作置位
来源：http://hz.jlsjyb.cn/gtgcifgegx.html

x |= (1 << 3);
来源：http://hz.hongshengwenyu.top/gtyqkswlyr.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtjyzrohmp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.havefunace.top/gthyepalsq.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gtkggcpbmk.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gthivyleqi.html

[S19] C：快速排序
来源：http://hz.zhongyouzk.top/gtapryiyto.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtnblejkik.html

[S20] C：二分查找
来源：http://hz.gogol.net.cn/gtmkrfidva.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtqfzluuzr.html

[S21] C：字符类别判断
来源：http://hz.zycfv.cn/gthdwkyhey.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gteerkogeg.html

[S22] C：字符串转数字
来源：http://hz.haohaochexian.top/gtqqhtbscp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtgxejjasq.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtkqjavjho.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tanke756.top/gtmbceyjni.html

[S24] C：获取本地时间
来源：http://hz.ydzc1.top/gtcxhbuusr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtpjaftvis.html

[S25] C：内存拷贝
来源：http://hz.ydzc1.top/gthgucctwd.html

memcpy(dst, src, n);
来源：http://hz.aizwys.cn/gttkqfowuz.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtnjdkpjzg.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigufen.top/gtzbktvtgp.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtwxfkcvxp.html

const double PI = 3.14159;
来源：http://hz.jianghu66.top/gthnubnkeu.html

[S28] C：静态变量
来源：http://hz.xingfuxueyuan.xyz/gtkuxsmgfr.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtgvhgugyl.html

[S29] C：变参函数
来源：http://hz.ywan-chungtsiang.top/gtxzhiekfp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gtrvudayoy.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtetxfodyh.html

#ifndef X_H
来源：http://hz.shuidangran.top/gtdyuslroj.html

#define X_H
来源：http://hz.zdqjudy.top/gtqhaszyvy.html

#endif
来源：http://hz.316326.xyz/gtnlpzlmhb.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtgyjexjty.html

#include <iostream>
来源：http://hz.jinyuanbaomall.cn/gtpehbyfuy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shuidangran.top/gtnmuwscbl.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtvnotgppq.html

std::string s = "hi";  s += "!";
来源：http://hz.pengpengdd.cyou/gtltstofbd.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtrzdoioun.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigufen.top/gtjpxgmbxm.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtnoadntjo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtgnudvkcq.html

[S35] C++：map
来源：http://hz.tianlin.xyz/gtylnaohas.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtwcrszfkw.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtgzonvhlm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtyrvsffvu.html

[S37] C++：set
来源：http://hz.ppjwa.cn/gtlraxnrsh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gtsxeiqbvd.html

[S38] C++：排序
来源：http://hz.redwolf501.top/gtzmhkkhvn.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtlivkfpts.html

[S39] C++：自定义比较器排序
来源：http://hz.cucudq.cn/gtyldcpfdt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtxvuoxksn.html

[S40] C++：查找元素
来源：http://hz.nwbrower.top/gtbfsukqib.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.redwolf501.top/gtacmrpocq.html

[S41] C++：类与构造函数
来源：http://hz.shzxlz.cn/gtchnysdni.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fzhhl.top/gtkaejydji.html

[S42] C++：继承与虚函数
来源：http://hz.hywenlv.cn/gtwgkxsdfd.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhongyouzk.top/gtmeimgald.html

[S43] C++：智能指针
来源：http://hz.cashguo.top/gtugkcvrba.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gtcsltnfdd.html

[S44] C++：引用传参
来源：http://hz.jinqigufen.top/gtnbrzkwkq.html

void inc(int &x) { ++x; }
来源：http://hz.shangyingyoupin.top/gtqxeswxvs.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gtbpnkcguu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ehwqpu.com/gtjwzhrolq.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtecbfjhnz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenzaomai.com/gtjzeadqjz.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gtkzipxmta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xingfuxueyuan.xyz/gtrcjjtqlj.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gtjhlwlsyb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cdnleiting.top/gtfcomhwrj.html

while (std::getline(in, line)) { }
来源：http://hz.yanxiufei.cn/gttykzpehe.html

[S49] C++：写文件
来源：http://hz.jinqigufen.top/gtmpdvodrl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gttcqfllqy.html

[S50] C++：格式化数字
来源：http://hz.ydjk.org.cn/gttxjueekn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinghuilouyu.cn/gtpkuvqxze.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtaqpcwpru.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtxhtllpvx.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtsqhjsswk.html

int size() const noexcept { return n_; }
来源：http://hz.ybcxt.top/gtdzclvcjq.html

[S53] C++：移动语义
来源：http://hz.sweek.top/gtzuyxxqxk.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtygudbevq.html

[S54] C++：异常处理
来源：http://hz.zdqjudy.top/gtvcnimwbg.html


<!-- 参考信息 -->