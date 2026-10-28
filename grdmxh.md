代发 wailian999

[Q76] 按天统计
来源：http://hz.hfpthk.cn/gtsydxgsle.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhengqikj.top/gtemvemawb.html

[Q77] 时间加减
来源：http://hz.0kj1m.cn/gttwncsibd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.feifeiyinyue.top/gtxklncoxo.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtinafkryh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aizwys.cn/gtdjsqgngo.html

[Q79] 字符串拼接
来源：http://hz.vqdsnc.cn/gtqorjwgqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.birdmap.top/gtqfrcndsa.html

[Q80] 字符串截取
来源：http://hz.zhengqikj.top/gtlwgucwxy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtifewsqxn.html

[Q81] 字符串替换
来源：http://hz.shuidangran.top/gtwzzsrexy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jianghu66.top/gthlllunwt.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtltefnosm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtulehhdac.html

[Q83] 大小写转换
来源：http://hz.chenlongwang.top/gthqmahahe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtofwxtjyj.html

[Q84] 去除首尾空格
来源：http://hz.nwbrower.top/gtnuortgoq.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuetiantiany.cn/gthutzmgpv.html

[Q85] 数值取整
来源：http://hz.ybcxt.top/gthognpvwf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pycfn.com/gtdgiecyho.html

[Q86] 读取 JSON 字段
来源：http://hz.ivvv.top/gtousjvxih.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xingfuxueyuan.xyz/gthitbtbmz.html

[Q87] JSON 字段做条件
来源：http://hz.aibaodan.cn/gtactrcsas.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hfpthk.cn/gtfqrtgbzm.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtsmjwbgad.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtpkhufhly.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhoulong.xyz/gtvysbolkc.html

[Q89] 判断表是否存在
来源：http://hz.52xcode.cn/gtrfqfjadq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xingfuxueyuan.xyz/gtuerbbxxq.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gtwjnnjxgo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tianlin.xyz/gtzxefbnwf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtatikybhq.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtlsyxyesj.html

================================================================================
来源：http://hz.ppjwa.cn/gthcmwpipn.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtnurevrjz.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtetqjlxmv.html

set -euo pipefail
来源：http://hz.havefunace.top/gtwvdvsiav.html

[R02] 变量赋值与使用
来源：http://hz.yuxming.cn/gtijjtfeqs.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtiqvqtwkh.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gthjufbrdc.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtcbfnaqmf.html

[R04] 位置参数
来源：http://hz.havefunace.top/gtbrckiwuy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.daria6918.cn/gtioqdsirk.html

[R05] 参数默认值
来源：http://hz.tanke756.top/gtvqjadisn.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtkzjbsnnw.html

[R06] 判断命令是否存在
来源：http://hz.9152youxi.cn/gtmbhylphm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gtktyrfevv.html

[R07] if 判断文件
来源：http://hz.jinqigufen.top/gtuddexhvo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yongpay.top/gtqkcddsug.html

[R08] 数值比较
来源：http://hz.fengsongda.top/gtljsdphur.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.meibo888.top/gtbffpiknu.html

[R09] 字符串比较
来源：http://hz.jianghu66.top/gtiuzlkzhz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gotoacloud.top/gtgvlgnygu.html

[R10] 正则匹配
来源：http://hz.zhiwuduotai.top/gtxvzxelbb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sysykeji.top/gtjaxbulxm.html

[R11] case 多分支
来源：http://hz.birdmap.top/gtgzozqusm.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtysacwtnh.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtmjvdqyrn.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtzqgdlnyn.html

*)     echo "未知命令" ;;
来源：http://hz.nanxuanxn.top/gtfrjzfmre.html

esac
来源：http://hz.wangshuangyany.cn/gtumdncthf.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtwcosrife.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtahwirrqm.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtiumpypcu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.mhx1999.top/gtolkgokqo.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gtnreknpuv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtiqgqdwoa.html

[R15] while 逐行读文件
来源：http://hz.feifeiyinyue.top/gtimqniikn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtsoyztbwf.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtkluxlkve.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gtebxluttu.html

[R17] 数组定义与取值
来源：http://hz.ppjwa.cn/gthtyfvdqi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.smart0.xyz/gtpnshfqnz.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gtredoxsge.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.9152youxi.cn/gtuhldsizk.html

[R19] 数组长度
来源：http://hz.yvedp.cn/gtmcquuecs.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtiihvdhbm.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtfijmbhpp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gtfcgzsksm.html

[R21] 字符串长度
来源：http://hz.zdqjudy.top/gtghprgeab.html

echo "${#s}"
来源：http://hz.cashguo.top/gtgxnxkgbk.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtwrhxmtgt.html

echo "${s:0:5}"
来源：http://hz.sweek.top/gtqhaudhgj.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gtljvussby.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtfrtnlvtr.html

[R24] 大小写转换
来源：http://hz.jqgufenzy.top/gtmdvhyodc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aibaodan.cn/gtclbqeeqd.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gttgksgaic.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinghuilouyu.cn/gtvwqmyfyb.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtmdlflrst.html

now=$(date +%F); echo "$now"
来源：http://hz.mhx1999.top/gtkckagzlt.html

[R27] 算术展开
来源：http://hz.316326.xyz/gtocgjzpkd.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gthnswkcga.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtrvbggxjz.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtdzbbzrfn.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtxevqugmm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gtexizaque.html

[R30] 函数返回状态码
来源：http://hz.zhiwuduotai.top/gtzciirifn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtszrlsflv.html

[R31] 局部变量
来源：http://hz.guowangkeji.top/gtavbebgjc.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtgcurrpse.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtmlrttaez.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gthcmtpurn.html

[R33] 捕获错误并提示行号
来源：http://hz.sxryk.cn/gtkkhnacfk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.andypj.xyz/gtncqzwcvv.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtgnrfvvqc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gttvgadjdf.html

[R35] 后台执行并等待
来源：http://hz.xingfuxueyuan.xyz/gtinhlgiig.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtyfevmtrt.html

[R36] 并发执行多个任务
来源：http://hz.zhengqikj.top/gtewawubcl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtzigagtfi.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtfmknotfk.html

files=$(ls -1)
来源：http://hz.316326.xyz/gtgnqruoyn.html

[R38] 管道串联
来源：http://hz.gzhubu.top/gtstsuvmhe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hammf.cn/gtywltdsoi.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtgcnsehfr.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtksvgvatk.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtnroudpak.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtfyqqkxrt.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtstpkjlxm.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtrlqitlmu.html

[R42] 输入重定向
来源：http://hz.vqdsnc.cn/gtrtevhigs.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtmeclkeyy.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtqfxkadql.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtrsnmjwnj.html

[R44] 按修改时间查找
来源：http://hz.guowangkeji.top/gtippbdkwy.html

find . -mtime -7 -type f
来源：http://hz.vqdsnc.cn/gtkrmobpfh.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gtualzlsnd.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gthbassnox.html

[R46] 递归替换文件内容
来源：http://hz.bjfxy.top/gthybegujx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gtetklgisq.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtyjumxzbq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtrjzbmklb.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gtidvblpks.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtehctibix.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtgxctbpnx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtfvgmgmtm.html

[R50] awk 求和
来源：http://hz.chenjidiqi.icu/gtlyywgxdn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shangyingyoupin.top/gtzmnleykn.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtxcdcewyg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aizwys.cn/gthgdbhnwt.html

[R52] 统计行数
来源：http://hz.guannengcc.top/gtdpnpucpn.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtjohxbpbj.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtwaecuipk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gtfqvgfane.html

[R54] 比较两个文件
来源：http://hz.birdmap.top/gtmnmxrbvu.html

diff a.txt b.txt
来源：http://hz.zhiwuduotai.top/gtrbqyxdsq.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtgkchexyq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtpyreodxn.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtqqcuifcv.html

scp file user@host:/path/
来源：http://hz.snrcjt.cn/gtgtvtpoxc.html

[R57] 远程执行命令
来源：http://hz.yongpay.top/gtapbtdque.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gtslcuvtgo.html

[R58] 下载文件
来源：http://hz.yj20258.top/gtiifoimkr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxinkj.top/gtgnfhxdpj.html

[R59] 发 POST JSON
来源：http://hz.zhixingplan.top/gtjkfxzoyb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gticgsrgdr.html

[R60] 只看 HTTP 状态码
来源：http://hz.cqqwz.cn/gtdmupodux.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jiagoushi.top/gtucyrhsdu.html

[R61] 磁盘占用
来源：http://hz.cucudq.cn/gtsozreidk.html

df -h;  du -sh *
来源：http://hz.fzhhl.top/gtvnmzztee.html

[R62] 找最占空间的文件
来源：http://hz.sufxvd.cn/gtsajkpkec.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gthilkzddj.html

[R63] 内存与进程
来源：http://hz.sxryk.cn/gtuldjvbim.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtuumlssdi.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtlhwiozed.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnxiangtu.top/gtxhszurfq.html

[R65] 查看端口占用
来源：http://hz.yangfankeji.com/gtfofrrtsl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydzc1.top/gtlbnrohba.html

[R66] 定时任务
来源：http://hz.fengsongda.top/gtesscutww.html

crontab -e;  crontab -l
来源：http://hz.sweek.top/gtbgphdvty.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gtdjeanufh.html

openssl rand -hex 16
来源：http://hz.ybcxt.top/gtzzepbyqn.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtwfuvdxer.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.smart0.xyz/gtrpnsnavq.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gtgbpknkiu.html

head -c 16 /dev/urandom | base64
来源：http://hz.yonumen.top/gtzyllyohr.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtfkkdfgva.html

date +%s;  date -d @1700000000
来源：http://hz.pycfn.com/gtkdluvfof.html

[R71] 日期格式化
来源：http://hz.smart0.xyz/gtbvwvihzy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtzdjggevs.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtkzelhohv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtedqfovdq.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtccrnotco.html

split -l 1000 big.log part_
来源：http://hz.jlsjyb.cn/gtfxjoxzed.html

[R74] 批量重命名
来源：http://hz.gotoacloud.top/gtiexdlbeu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fengsongda.top/gttvagwtob.html

[R75] 导出环境变量
来源：http://hz.shangyingyoupin.top/gtxbpjxpet.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xinyue.icu/gtbpmnpswk.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangtech.top/gtuchvfvrj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gthaeuvchr.html

[R77] 读取用户输入
来源：http://hz.zhijiandao.cn/gtawhiwdtj.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtfnpangwi.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtgwrvutqh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gthiuthjjz.html

[R79] 解析命令行选项
来源：http://hz.ydzc1.top/gtkfhoyvxs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj20258888.top/gttirzkouw.html

[R80] 查看脚本执行耗时
来源：http://hz.sysykeji.top/gtpkhimnmx.html

time ./run.sh
来源：http://hz.chenjidiqi.icu/gttfvzhfjb.html

================================================================================
来源：http://hz.hfpthk.cn/gtjvnimsia.html

S. C / C++ 专题
来源：http://hz.jlsjyb.cn/gthyrppeuy.html

================================================================================
来源：http://hz.gaohongyu789.top/gteagnrvzp.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gtitzkxcvk.html

#include <stdio.h>
来源：http://hz.shzxlz.cn/gtnriqyckq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jiagoushi.top/gtrdviqvwu.html

[S02] C：变量与格式化输出
来源：http://hz.dianchejie.cn/gtfikpimbr.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gtvrhtfbgk.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gtbvrogska.html

int x; scanf("%d", &x);
来源：http://hz.sxryk.cn/gtrvfsrcaz.html

[S04] C：字符串复制
来源：http://hz.yanxiufei.cn/gtpletffdv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtpvqmgdxo.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtbdtaryxt.html

strlen(s)
来源：http://hz.shangyingyoupin.top/gtcnkipxna.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtqjhrwarz.html

strcmp(a, b) == 0
来源：http://hz.redwolf501.top/gtjyehvcco.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gttepmdkgb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhoulong.xyz/gtbqwbmmlq.html

[S08] C：动态内存分配与释放
来源：http://hz.hnxiangtu.top/gtyqrqinrw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gzhubu.top/gtqjjgxfff.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtctaiabtl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gzhubu.top/gtbwutswwt.html

[S10] C：指针与解引用
来源：http://hz.52xcode.cn/gtspuppseu.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtrqlviuhy.html

[S11] C：逐行读文件
来源：http://hz.svipenyu.cn/gtmjohxmgd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhijiandao.cn/gtzgelckll.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtessjxgwh.html

fclose(f);
来源：http://hz.ydjk.org.cn/gtzgkspowj.html

[S12] C：写文件
来源：http://hz.fzhhl.top/gtltmxucqs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gtfpcpawpp.html

[S13] C：宏定义
来源：http://hz.mhx1999.top/gtfwsoreav.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jyoumei.cn/gtmcobfvdx.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtiernsvyp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ybcxt.top/gtbwmqinhw.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtfhkidjps.html

(double) a / b
来源：http://hz.yonumen.top/gtdcdepihk.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtejvjymkb.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gtccvlvdlg.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258.top/gtiukmwwot.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtukutynlb.html

[S18] C：命令行参数
来源：http://hz.andypj.xyz/gtpeoyiktd.html

int main(int argc, char **argv)
来源：http://hz.316326.xyz/gtfobwtuli.html

[S19] C：快速排序
来源：http://hz.feifeiyinyue.top/gtquuokhsi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtpoifaxhr.html

[S20] C：二分查找
来源：http://hz.gzhubu.top/gtowregekw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtwwikbich.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gtwhpbyker.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtkhinxbhd.html

[S22] C：字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtjmkdqihz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtbhsivars.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtmcndbekm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigfzy.top/gtdlgaikpp.html

[S24] C：获取本地时间
来源：http://hz.ywan-chungtsiang.top/gtizkcofwk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtawpliuda.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtaqynlqpi.html

memcpy(dst, src, n);
来源：http://hz.redwolf501.top/gtqmkljnit.html

[S26] C：内存清零
来源：http://hz.zhoulong.xyz/gttbtqceox.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtkswdndtw.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtrhrfcogd.html

const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtposgwnjf.html

[S28] C：静态变量
来源：http://hz.xylfe.cn/gttfzlaegx.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtiujaqemj.html

[S29] C：变参函数
来源：http://hz.yongpay.top/gtayobbiys.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtxhqikedm.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gttusistde.html

#ifndef X_H
来源：http://hz.xinyue.icu/gthuxnrshx.html

#define X_H
来源：http://hz.tianlin.xyz/gtihiyxjxg.html

#endif
来源：http://hz.gzhubu.top/gtddfozdud.html

[S31] C++：Hello World
来源：http://hz.ywan-chungtsiang.top/gtdtiksxtj.html

#include <iostream>
来源：http://hz.chenzaomai.com/gthamdpscg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenzaomai.com/gtfwkkmlls.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtfjjayizw.html

std::string s = "hi";  s += "!";
来源：http://hz.daxiang520.top/gtzrxnuxnq.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtqokhdpew.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sysykeji.top/gtmpowkxww.html

[S34] C++：遍历 vector
来源：http://hz.nanxinkj.top/gtuqnbscjo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.havefunace.top/gtwyvnjhvt.html

[S35] C++：map
来源：http://hz.hywenlv.cn/gtkxlcrwgj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtuwvypdbc.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gtagwzutnl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtkotvwcwg.html

[S37] C++：set
来源：http://hz.jqgfzy.top/gtprofrsab.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.c1oappe.top/gtlfqnqhmh.html

[S38] C++：排序
来源：http://hz.sweek.top/gtmmhvdqsn.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gtgzpfpkby.html

[S39] C++：自定义比较器排序
来源：http://hz.xuetiantiany.cn/gtjqlfopsd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtokndrnih.html

[S40] C++：查找元素
来源：http://hz.pengpengdd.cyou/gtfpexhzoy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtcjaprufv.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gtkwkeravm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yongpay.top/gtvdwpgytr.html

[S42] C++：继承与虚函数
来源：http://hz.hywenlv.cn/gttiykolzr.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gttfopftni.html

[S43] C++：智能指针
来源：http://hz.c1oappe.top/gtwlijplws.html

auto p = std::make_unique<int>(5);
来源：http://hz.gotoacloud.top/gtbdnqaerp.html

[S44] C++：引用传参
来源：http://hz.hfpthk.cn/gtrxuunaqm.html

void inc(int &x) { ++x; }
来源：http://hz.jiagoushi.top/gteujnfvvy.html

[S45] C++：lambda
来源：http://hz.gzhubu.top/gtheeqzkak.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtzlybohzg.html

[S46] C++：函数模板
来源：http://hz.sweek.top/gtrjawyyss.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gtfjjajltp.html


<!-- 参考信息 -->