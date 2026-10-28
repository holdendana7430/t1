代发 wailian999

[Q78] 当前时间
来源：http://hz.kuanghao11.cn/gtfrmorzhp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gtycchdocw.html

[Q79] 字符串拼接
来源：http://hz.316326.xyz/gtovuetneq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ywan-chungtsiang.top/gtqrrdedcz.html

[Q80] 字符串截取
来源：http://hz.wangshuangyany.cn/gtzkujhcdk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtxyxveqan.html

[Q81] 字符串替换
来源：http://hz.smart0.xyz/gtuzwznasb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hongshengwenyu.top/gtcilycmym.html

[Q82] 字符长度与字节长度
来源：http://hz.ydzc1.top/gtqpemfsts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gtncyjecdo.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtijbgmpqj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgufenzy.top/gtqrawyuwa.html

[Q84] 去除首尾空格
来源：http://hz.jqgufenzy.top/gtmtyhiyel.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtpwxshjcn.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gttlrssluj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtpylxmxvc.html

[Q86] 读取 JSON 字段
来源：http://hz.hfpthk.cn/gthlwlmpgt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinyuanbaomall.cn/gtqsesfcpk.html

[Q87] JSON 字段做条件
来源：http://hz.tianlin.xyz/gtsjheukvk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.iojbl.cn/gtbyuwvfsc.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtbxdjqihv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jiagoushi.top/gtbnmiqcgr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cheryme.top/gtxqxjuqje.html

[Q89] 判断表是否存在
来源：http://hz.smart0.xyz/gtvqudzxrx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gtxrxrpzcl.html

[Q90] 生成序号列
来源：http://hz.aibaodan.cn/gtfctgembp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtrjwffcip.html

================================================================================
来源：http://hz.nwbrower.top/gtsfdcnztm.html

R. Bash 专题
来源：http://hz.gotoacloud.top/gtubhosjtq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdbaqwemo.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gttircewcm.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gturachbuv.html

set -euo pipefail
来源：http://hz.ppjwa.cn/gtwzminbmb.html

[R02] 变量赋值与使用
来源：http://hz.hnqzz.top/gtmnpoqoip.html

name="Tom"; echo "$name"
来源：http://hz.sysykeji.top/gtmvjywkbg.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtlunlhspa.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gtyoccmgou.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gthtbwfjko.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtwfwyidwf.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtpkesysmh.html

name="${1:-default}"
来源：http://hz.havefunace.top/gtqiyhgfag.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtecxkqeuw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gtjcnhyjeg.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtfeixfdwf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtzcdaibox.html

[R08] 数值比较
来源：http://hz.sxryk.cn/gtoffdcymr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gtdsmxhanc.html

[R09] 字符串比较
来源：http://hz.shanyushiyangtech.top/gtkrqsaggt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fengsongda.top/gtqbdjdtws.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtqefseumo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtdqcmyzkr.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtowqegvcd.html

case "$1" in
来源：http://hz.cdnleiting.top/gtnnoeduza.html

start) echo "启动" ;;
来源：http://hz.chenjidiqi.icu/gtpkjcrdtr.html

stop)  echo "停止" ;;
来源：http://hz.jyoumei.cn/gtgjklxjod.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtvskhljgq.html

esac
来源：http://hz.guowangkeji.top/gtqlztvhbc.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtcskgxyvy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangshuangyany.cn/gtsitqinjn.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtesryjbms.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cdnleiting.top/gtkuczfryf.html

[R14] C 风格 for
来源：http://hz.yangfankeji.com/gteucmtctn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtznublxdv.html

[R15] while 逐行读文件
来源：http://hz.daria6918.cn/gtrcrdqsmm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.svipenyu.cn/gtlmfoyvxh.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtrgeoytsd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtjbpfvtgl.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtqbikfnrj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtmlstfziq.html

[R18] 遍历数组
来源：http://hz.wangdashe.top/gtuflvoond.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gtahqlobal.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtjfusfcqf.html

echo "${#arr[@]}"
来源：http://hz.sufxvd.cn/gtityxkawo.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtasxkremk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xingfuxueyuan.xyz/gtjqhffnnk.html

[R21] 字符串长度
来源：http://hz.jianghu66.top/gthnjndldv.html

echo "${#s}"
来源：http://hz.tianlin.xyz/gthvjktnlj.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gtfxcxozhp.html

echo "${s:0:5}"
来源：http://hz.haohaochexian.top/gtayukujdi.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtowxxoiqk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtestrqhty.html

[R24] 大小写转换
来源：http://hz.cucudq.cn/gtyvqixdte.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhaomingkeji.xyz/gtamccbuin.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtobyqzjcn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuanzx.com/gtwaslfswt.html

[R26] 命令替换
来源：http://hz.xziqi.cn/gtszleutax.html

now=$(date +%F); echo "$now"
来源：http://hz.xuetiantiany.cn/gtuskxgcni.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtdldkjqjk.html

echo $((1 + 2 * 3))
来源：http://hz.aizwys.cn/gtzhyuilsy.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtjcqslykc.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtdcngcdlr.html

[R29] 定义函数
来源：http://hz.iojbl.cn/gtgfxrgwwy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gaohongyu789.top/gtautektbq.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtjydkwlod.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigufen.top/gtqrmpanea.html

[R31] 局部变量
来源：http://hz.zhaomingkeji.xyz/gtwfutwuci.html

f() { local x=1; echo "$x"; }
来源：http://hz.guowangkeji.top/gtmwaovatl.html

[R32] 参数个数校验
来源：http://hz.zhixingplan.top/gtoijuazys.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.9152youxi.cn/gtxeudixam.html

[R33] 捕获错误并提示行号
来源：http://hz.gzhubu.top/gtkxoahujp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.mhx1999.top/gtkraqrskt.html

[R34] 退出时清理
来源：http://hz.jlsjyb.cn/gtamdbcqen.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtaclyetyj.html

[R35] 后台执行并等待
来源：http://hz.guannengcc.top/gtlxqdieqf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hammf.cn/gtxxfesecf.html

[R36] 并发执行多个任务
来源：http://hz.birdmap.top/gtnjdbvsky.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj202588.top/gtdzcflpwu.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtbhncqchc.html

files=$(ls -1)
来源：http://hz.bjfxy.top/gtrgzwhldw.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtmdmiapdd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtegmfezli.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtnhnhflhf.html

cmd > out.log 2>&1
来源：http://hz.yonumen.top/gtrwxokopd.html

[R40] 追加写日志
来源：http://hz.sxryk.cn/gtdvlntowc.html

echo "log" >> out.log
来源：http://hz.chenzaomai.com/gtgwisfzfo.html

[R41] 丢弃输出
来源：http://hz.ppjwa.cn/gtdzgsdcsm.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258.top/gtnauvjpyp.html

[R42] 输入重定向
来源：http://hz.jqgfzy.top/gtgsxkbyey.html

wc -l < a.txt
来源：http://hz.chenlongwang.top/gthjocuqfu.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gtbnblvdyv.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtjnvdljkk.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gttpjvjyac.html

find . -mtime -7 -type f
来源：http://hz.tian-w.cn/gtiyjcklig.html

[R45] 批量删除
来源：http://hz.meibo888.top/gtzsonpwfm.html

find . -name "*.tmp" -delete
来源：http://hz.9152youxi.cn/gtopkojlik.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtqekhgbba.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhaomingkeji.xyz/gtiilkclhx.html

[R47] sed 单行替换
来源：http://hz.cheryme.top/gthyprrobm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtuolyrsye.html

[R48] awk 取指定列
来源：http://hz.svipenyu.cn/gtvxuwdamz.html

awk '{print $1, $3}' a.txt
来源：http://hz.gotoacloud.top/gtnhgnsapw.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gteulsfspq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yueranfly.top/gtbutskmts.html

[R50] awk 求和
来源：http://hz.jqgfzy.top/gtgyhwmotl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ybcxt.top/gtjkwxjsto.html

[R51] 排序去重取前几
来源：http://hz.smart0.xyz/gtpzqgaagg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtpejmgcfb.html

[R52] 统计行数
来源：http://hz.jinqigufen.top/gtsrezdbup.html

wc -l a.txt
来源：http://hz.guowangkeji.top/gtzjsgjbps.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtodayjhde.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangkeji.top/gtfnthvlfm.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtnrbyoiwi.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtjubptohd.html

[R55] 压缩与解压
来源：http://hz.chenlongwang.top/gtljctvajo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gotoacloud.top/gtojpnraru.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtvcorxazu.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtckjjwqlr.html

[R57] 远程执行命令
来源：http://hz.zhixingplan.top/gtrqxhbvos.html

ssh user@host 'uptime'
来源：http://hz.tanke756.top/gtqelonkat.html

[R58] 下载文件
来源：http://hz.jinyuanbaomall.cn/gtylhwdoxj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tianlin.xyz/gtgivcuptt.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtavbphbdo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yueranfly.top/gtkmvgwmvx.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtlqximenk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zdqjudy.top/gteowiwhph.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtiupzadzi.html

df -h;  du -sh *
来源：http://hz.cashguo.top/gtrfvssjjw.html

[R62] 找最占空间的文件
来源：http://hz.birdmap.top/gtbzqybkkz.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtxunnjuel.html

[R63] 内存与进程
来源：http://hz.yanxiufei.cn/gtezbhrfef.html

free -h;  ps aux | grep nginx
来源：http://hz.jiagoushi.top/gtgqqrtzms.html

[R64] 结束进程
来源：http://hz.zhongyouzk.top/gtlnegkccq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.quarkkingdee.top/gtzzppeyfs.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtkwotjnuz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yanxiufei.cn/gtilywbbvu.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gthvmcfdzd.html

crontab -e;  crontab -l
来源：http://hz.chenzaomai.com/gtespwduza.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gteumfpdtd.html

openssl rand -hex 16
来源：http://hz.0kj1m.cn/gtppsvnlbt.html

[R68] 计算文件校验值
来源：http://hz.tianlin.xyz/gtlebvnyin.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.52xcode.cn/gtcufuokud.html

[R69] 生成随机密码
来源：http://hz.hysaishi.cn/gtyyketdiw.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtimvzbsgn.html

[R70] 时间戳与互转
来源：http://hz.birdmap.top/gthypeyjcr.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gtvajjaqbl.html

[R71] 日期格式化
来源：http://hz.sufxvd.cn/gtnhajfhfp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhongyouzk.top/gtxlfcuaxd.html

[R72] 等待端口就绪
来源：http://hz.hywenlv.cn/gthmidwjnd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtfheaepbs.html

[R73] 分割大日志
来源：http://hz.kuanghao11.cn/gtfwljqdxg.html

split -l 1000 big.log part_
来源：http://hz.kuanghao11.cn/gtxnvgwwuk.html

[R74] 批量重命名
来源：http://hz.dashuyun.cn/gtkevhiaff.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnqzz.top/gtfhounhgu.html

[R75] 导出环境变量
来源：http://hz.dashuyun.cn/gtndraygoq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gtaoyunqci.html

[R76] 使用临时文件
来源：http://hz.316326.xyz/gtrwhawbwj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtujmtyigp.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtlcpcqiqo.html

read -rp "请输入: " ans
来源：http://hz.bjfxy.top/gtilthbijb.html

[R78] 交互式菜单
来源：http://hz.xinyue.icu/gtbpdcbdon.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtneeezwob.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtlynwzkgi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhijiandao.cn/gtypawbeyh.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtapzrfumn.html

time ./run.sh
来源：http://hz.shzxlz.cn/gtyjcybyiw.html

================================================================================
来源：http://hz.shuidangran.top/gtyrwxwscs.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gtwtzlpson.html

================================================================================
来源：http://hz.aizwys.cn/gtovcxzosy.html

[S01] C：Hello World
来源：http://hz.tanke756.top/gtcyjqlxlz.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtyjfvthtn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydjk.org.cn/gthzghpxcu.html

[S02] C：变量与格式化输出
来源：http://hz.birdmap.top/gtvkmkcknx.html

int a = 10; printf("%d\n", a);
来源：http://hz.jiagoushi.top/gtzunawyvt.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gthgwlrory.html

int x; scanf("%d", &x);
来源：http://hz.jyoumei.cn/gthdmfbhly.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtqozsdezo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtnfjtmqjv.html

[S05] C：字符串长度
来源：http://hz.xuetiantiany.cn/gtfqygkcnm.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtxuazbens.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangkeji.top/gtphnqrqjg.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtvevralvf.html

[S07] C：数组遍历求和
来源：http://hz.jinyuanbaomall.cn/gtizsnezyl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxuanxn.top/gtkdnhjqhd.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtazjvacsy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cashguo.top/gtgvjpxhab.html

[S09] C：结构体定义与初始化
来源：http://hz.daria6918.cn/gtmapltszw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yongpay.top/gtwwlsyjqz.html

[S10] C：指针与解引用
来源：http://hz.jinqigfzy.top/gtljdxzayp.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangtech.top/gtsckoslfj.html

[S11] C：逐行读文件
来源：http://hz.yj20258888.top/gtkfmpxdpd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.feifeiyinyue.top/gtkioqfmcl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xziqi.cn/gtadruhcle.html

fclose(f);
来源：http://hz.hnxiangtu.top/gtjtpeiczk.html

[S12] C：写文件
来源：http://hz.jianghu66.top/gtkpwfdfqc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gticbxozub.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtxsghctwu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zycfv.cn/gtkenuwtfw.html

[S14] C：枚举
来源：http://hz.yueranfly.top/gtthcqbrnf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtvwvexkkt.html

[S15] C：类型转换
来源：http://hz.pycfn.com/gtuksgarph.html

(double) a / b
来源：http://hz.nwbrower.top/gtkpwhvcdv.html

[S16] C：位操作置位
来源：http://hz.ydzc1.top/gtilbwbqrp.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtlbaclzlv.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gtbovmyvaw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jlsjyb.cn/gtaptpyidj.html

[S18] C：命令行参数
来源：http://hz.nanxuanxn.top/gthvxwzkmz.html

int main(int argc, char **argv)
来源：http://hz.xylfe.cn/gttlshhcmu.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtqrfcuquw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gtgqbdmqzk.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtznvywfls.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtybuswunf.html

[S21] C：字符类别判断
来源：http://hz.hfpthk.cn/gtbzjlblpz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cashguo.top/gtrkdqcmdm.html

[S22] C：字符串转数字
来源：http://hz.haohaochexian.top/gtetzhiyad.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gtpucybpqx.html

[S23] C：随机数
来源：http://hz.ybcxt.top/gttyydkhvd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtylnpkebn.html

[S24] C：获取本地时间
来源：http://hz.bjfxy.top/gtuodnsnnq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangshuangyany.cn/gtgmhkckmf.html

[S25] C：内存拷贝
来源：http://hz.guowangkeji.top/gttwcwnfbc.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtlpkxwdqa.html

[S26] C：内存清零
来源：http://hz.xziqi.cn/gtzyyptzcg.html

memset(a, 0, sizeof a);
来源：http://hz.pycfn.com/gtyorutxpt.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gthoipuzvp.html

const double PI = 3.14159;
来源：http://hz.gogol.net.cn/gtkswwspez.html

[S28] C：静态变量
来源：http://hz.hywenlv.cn/gtwkvpskgk.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtwnnzabdl.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtbpelmxga.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydjk.org.cn/gtvfaembca.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtrnxsoaku.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtnkdyqvrh.html

#define X_H
来源：http://hz.zhongyouzk.top/gtldkcgmfy.html

#endif
来源：http://hz.mhx1999.top/gtodljibnk.html

[S31] C++：Hello World
来源：http://hz.chenjidiqi.icu/gteqgoiovi.html

#include <iostream>
来源：http://hz.tianlin.xyz/gtfkphbrva.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xinyue.icu/gtcljzfvyy.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtmqytoeaf.html

std::string s = "hi";  s += "!";
来源：http://hz.gzhubu.top/gtksxhsjap.html

[S33] C++：vector 增删
来源：http://hz.jqgfzy.top/gtdxlwtjoy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gthnrvnmes.html

[S34] C++：遍历 vector
来源：http://hz.xingfuxueyuan.xyz/gtqprmxyxw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtooblobsg.html

[S35] C++：map
来源：http://hz.hongshengwenyu.top/gtbhrxftwr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtolzielfc.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gtyjyykxih.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtduskenzv.html

[S37] C++：set
来源：http://hz.ivvv.top/gttgoghnfb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hysaishi.cn/gtnhwrgtfh.html

[S38] C++：排序
来源：http://hz.ydzc1.top/gthugcydss.html

std::sort(v.begin(), v.end());
来源：http://hz.guowangkeji.top/gthaijvdjw.html

[S39] C++：自定义比较器排序
来源：http://hz.ppjwa.cn/gtghgbqhmd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtbjayduzo.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtzmowwpuu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtnznawvry.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gttfkmaegv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigfzy.top/gtahbyytwh.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtowimqcis.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuetiantiany.cn/gtunowstgy.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtqyqipial.html

auto p = std::make_unique<int>(5);
来源：http://hz.nwbrower.top/gttnpoavif.html

[S44] C++：引用传参
来源：http://hz.iojbl.cn/gtwbesafqd.html

void inc(int &x) { ++x; }
来源：http://hz.vqdsnc.cn/gtzijdvuyq.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtjlsdikgg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.vqdsnc.cn/gtdtchyrfv.html

[S46] C++：函数模板
来源：http://hz.mhx1999.top/gtrudnxrzl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gzhubu.top/gtgldoormx.html

[S47] C++：结构化绑定遍历
来源：http://hz.jyoumei.cn/gtulxrdgio.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.bjfxy.top/gtorojotnv.html

[S48] C++：逐行读文件
来源：http://hz.jiagoushi.top/gtnahbtfxf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgufenzy.top/gtjhygrtkg.html


<!-- 参考信息 -->