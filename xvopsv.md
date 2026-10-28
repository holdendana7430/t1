代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtorfxakrl.html

[Q75] 日期格式化
来源：http://hz.ppjwa.cn/gtrcuwuvqs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.c1oappe.top/gtfggzarah.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtkklbaihh.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtpypyuqoo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenjidiqi.icu/gtzkxkbbqd.html

[Q77] 时间加减
来源：http://hz.zhengqikj.top/gtwcxsxoqz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.mhx1999.top/gtsszmpvzw.html

[Q78] 当前时间
来源：http://hz.316326.xyz/gtzdnmzztb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnxiangtu.top/gtvigbzyru.html

[Q79] 字符串拼接
来源：http://hz.zhijiandao.cn/gtbdcceqnv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.52xcode.cn/gtvhnqgonl.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtgeslawaq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuanzx.com/gtravbjdkq.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtksmrutqh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.svipenyu.cn/gtvivszxlq.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtwuvqutgk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtvhbjxpwd.html

[Q83] 大小写转换
来源：http://hz.guowangkeji.top/gtmzfpzspr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jlsjyb.cn/gtxjksgvbp.html

[Q84] 去除首尾空格
来源：http://hz.tian-w.cn/gtoxvqrsak.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydzc1.top/gteqwqazbg.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gtxixhrspj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtasrfsqvf.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtivysrydd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gzhubu.top/gtixhisnrj.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gtrekfzmrb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jianghu66.top/gthhmhrodn.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtikxdgvwk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtodpzhckh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.svipenyu.cn/gtzhuahscb.html

[Q89] 判断表是否存在
来源：http://hz.bjfxy.top/gtvjmvdful.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtkzupgzdt.html

[Q90] 生成序号列
来源：http://hz.dashuyun.cn/gtqvevqara.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhiwuduotai.top/gtzxkumxll.html

================================================================================
来源：http://hz.nanxinkj.top/gtptetsllp.html

R. Bash 专题
来源：http://hz.dashuyun.cn/gtdfamtjrf.html

================================================================================
来源：http://hz.xziqi.cn/gttpuptldt.html

[R01] shebang 与严格模式
来源：http://hz.gzhubu.top/gtmdtrmeod.html

#!/usr/bin/env bash
来源：http://hz.daxiang520.top/gtrvkzlutz.html

set -euo pipefail
来源：http://hz.shuidangran.top/gtmiwphhts.html

[R02] 变量赋值与使用
来源：http://hz.9152youxi.cn/gtquncagku.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gttiimeirn.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtymqrzygf.html

readonly PI=3.14
来源：http://hz.guowangkeji.top/gtdkhprpsv.html

[R04] 位置参数
来源：http://hz.haohaochexian.top/gtohznqdsr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtscxskgtf.html

[R05] 参数默认值
来源：http://hz.jqgufenzy.top/gtstgdviva.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtsaqkknit.html

[R06] 判断命令是否存在
来源：http://hz.chenzaomai.com/gtsemzeqxy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtuoyvkpdb.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtfojrvvkx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gtmgdljcnw.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtrrpkailh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtvstnsmtj.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtzxvzhajw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhongyouzk.top/gtjpfzfacu.html

[R10] 正则匹配
来源：http://hz.ehwqpu.com/gtkraowjof.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangtech.top/gtxyrzltrf.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gtwgssjmwj.html

case "$1" in
来源：http://hz.sweek.top/gtkbkozqjx.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtvqdfswof.html

stop)  echo "停止" ;;
来源：http://hz.tanke756.top/gtimnpbgzg.html

*)     echo "未知命令" ;;
来源：http://hz.hnxiangtu.top/gtetzxcxto.html

esac
来源：http://hz.shanyushiyangkeji.top/gtnlvqdffz.html

[R12] for 遍历文件
来源：http://hz.xziqi.cn/gtjaizqzun.html

for f in *.txt; do echo "$f"; done
来源：http://hz.snrcjt.cn/gtifluygcc.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtxxjbzotw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yvedp.cn/gtvibgsjhw.html

[R14] C 风格 for
来源：http://hz.aibaodan.cn/gtfdszzqqw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gtujewjiuq.html

[R15] while 逐行读文件
来源：http://hz.chenjidiqi.icu/gtulpjqmko.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtwwjpctma.html

[R16] until 等待条件
来源：http://hz.hnxiangtu.top/gtdwnyishq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.redwolf501.top/gteweamrdd.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtxcdgokcp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ywan-chungtsiang.top/gtwdpnljnp.html

[R18] 遍历数组
来源：http://hz.quarkkingdee.top/gtqveocqzt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.haohaochexian.top/gttekjpdys.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtlerasmvt.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtbxpboijf.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtanidxyyv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnxiangtu.top/gtqbvmrjqg.html

[R21] 字符串长度
来源：http://hz.shanyushiyangkeji.top/gtrvkzhktt.html

echo "${#s}"
来源：http://hz.jyoumei.cn/gtfgrwbzwh.html

[R22] 截取子串
来源：http://hz.havefunace.top/gtnwyqtivv.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gtdyzowmeo.html

[R23] 字符串替换
来源：http://hz.cashguo.top/gtulcctmzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ppjwa.cn/gthgdkermd.html

[R24] 大小写转换
来源：http://hz.snrcjt.cn/gtsabafgkb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.smart0.xyz/gthjjqrdva.html

[R25] 去后缀 / 去前缀
来源：http://hz.yueranfly.top/gtcpkcqrxo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.9152youxi.cn/gtatoinhni.html

[R26] 命令替换
来源：http://hz.jinyuanbaomall.cn/gthbybsikm.html

now=$(date +%F); echo "$now"
来源：http://hz.ydjk.org.cn/gtllhxxxcl.html

[R27] 算术展开
来源：http://hz.fengsongda.top/gtmokjvjcb.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtodzyneci.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtzglqvshn.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gtbeymnhom.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtgjiqxioz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtttwdkmsz.html

[R30] 函数返回状态码
来源：http://hz.zhongyouzk.top/gthkxqbpcq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtcxpopogp.html

[R31] 局部变量
来源：http://hz.nwbrower.top/gtqiygmakv.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gttgjdqwna.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtydohargb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxuanxn.top/gteftahroq.html

[R33] 捕获错误并提示行号
来源：http://hz.tian-w.cn/gtzbybokkv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gotoacloud.top/gtcruabjdd.html

[R34] 退出时清理
来源：http://hz.zhengqikj.top/gtieysqiiz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtbpzuuilu.html

[R35] 后台执行并等待
来源：http://hz.yanxiufei.cn/gtjlpzefex.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangkeji.top/gthulsviya.html

[R36] 并发执行多个任务
来源：http://hz.hfpthk.cn/gtjcpzpfvl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigufen.top/gtytleublk.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtxjfuwquj.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtdptmiozm.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtqpybjgrh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtoywxnxdb.html

[R39] 重定向标准输出与错误
来源：http://hz.zhijiandao.cn/gtqwgupugm.html

cmd > out.log 2>&1
来源：http://hz.jlsjyb.cn/gtgmxnhudz.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtxlycbphl.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtdqekvnmh.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtutjvesro.html

cmd >/dev/null 2>&1
来源：http://hz.xylfe.cn/gtoadrxyyv.html

[R42] 输入重定向
来源：http://hz.gzhubu.top/gtdncshtag.html

wc -l < a.txt
来源：http://hz.svipenyu.cn/gtofymtvgb.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtupbjownk.html

find . -name "*.log" -type f
来源：http://hz.gaohongyu789.top/gtsdubzfyl.html

[R44] 按修改时间查找
来源：http://hz.chenjidiqi.icu/gtuzjmjpjp.html

find . -mtime -7 -type f
来源：http://hz.pengpengdd.cyou/gtdcilthbk.html

[R45] 批量删除
来源：http://hz.daxiang520.top/gtvnovbrbh.html

find . -name "*.tmp" -delete
来源：http://hz.gotoacloud.top/gtndgzphpc.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtoyxvnkzk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zdqjudy.top/gtpdmpqvva.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtwixzeqsc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hywenlv.cn/gtdmhnapxf.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gticugclzm.html

awk '{print $1, $3}' a.txt
来源：http://hz.gogol.net.cn/gtgforkmyi.html

[R49] awk 带条件
来源：http://hz.52xcode.cn/gtancqjxrm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtjjwsxvyi.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtourucpxj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pycfn.com/gtftagiixv.html

[R51] 排序去重取前几
来源：http://hz.nanxinkj.top/gtzpxepxsx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gtbgumwtxf.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtnejzlxhr.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtmnbgrrmg.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtltrmqdag.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.vqdsnc.cn/gtplejrbua.html

[R54] 比较两个文件
来源：http://hz.xuanzx.com/gtlufncnue.html

diff a.txt b.txt
来源：http://hz.jinghuilouyu.cn/gtiwgdtaib.html

[R55] 压缩与解压
来源：http://hz.quarkkingdee.top/gtcmvqxptc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yvedp.cn/gtlpamnnnc.html

[R56] 远程拷贝
来源：http://hz.gotoacloud.top/gtdcwaadgw.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtcnegvjzd.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtpbqgxdxn.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtqubcowfq.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gttlbjgxcu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgfzy.top/gtxpeocrvd.html

[R59] 发 POST JSON
来源：http://hz.zhixingplan.top/gtcplrffkn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.guowangkeji.top/gtieryzxjr.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtvojhfiuw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.svipenyu.cn/gtyaibmzio.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gtkzbgnoqh.html

df -h;  du -sh *
来源：http://hz.yuxming.cn/gtbizvxofy.html

[R62] 找最占空间的文件
来源：http://hz.chenzaomai.com/gtdzrfsjsh.html

du -ah . | sort -rh | head -10
来源：http://hz.andypj.xyz/gtnasbrjja.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtmrwttwhk.html

free -h;  ps aux | grep nginx
来源：http://hz.gotoacloud.top/gtpqbnzeys.html

[R64] 结束进程
来源：http://hz.mhx1999.top/gtgeqmjiyk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zycfv.cn/gtvglrxrqm.html

[R65] 查看端口占用
来源：http://hz.jqgfzy.top/gtrkzdhvud.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtjrnpikfn.html

[R66] 定时任务
来源：http://hz.xingfuxueyuan.xyz/gtefxfothi.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtpzqqdfaa.html

[R67] 生成随机十六进制串
来源：http://hz.yuxming.cn/gthlojdicg.html

openssl rand -hex 16
来源：http://hz.hammf.cn/gtkuqrhjea.html

[R68] 计算文件校验值
来源：http://hz.quarkkingdee.top/gtnpndikun.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.birdmap.top/gtzacsylnn.html

[R69] 生成随机密码
来源：http://hz.ybcxt.top/gtdhfabjiq.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtmzcyeips.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtoarhkniw.html

date +%s;  date -d @1700000000
来源：http://hz.xylfe.cn/gtqgovwinv.html

[R71] 日期格式化
来源：http://hz.bjfxy.top/gticrrennz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtwjtvzdyh.html

[R72] 等待端口就绪
来源：http://hz.sweek.top/gtwrfnnfvu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtulwehrcd.html

[R73] 分割大日志
来源：http://hz.yj202588.top/gtqoktsfrm.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtayvbflwg.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtmupyxpbc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gttgwmbwve.html

[R75] 导出环境变量
来源：http://hz.ppjwa.cn/gtjwmgkfuy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtzknxvilc.html

[R76] 使用临时文件
来源：http://hz.zycfv.cn/gtkbjjtbfa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fzhhl.top/gtnrixucen.html

[R77] 读取用户输入
来源：http://hz.hywenlv.cn/gtpszytpqv.html

read -rp "请输入: " ans
来源：http://hz.sweek.top/gtmpghsvfl.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtrgjuvotf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jlsjyb.cn/gttexapmwd.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtxbndaphy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj202588.top/gtioaokscr.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtmvcxsegp.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtpfwhsqxa.html

================================================================================
来源：http://hz.tanke756.top/gtufjxgiom.html

S. C / C++ 专题
来源：http://hz.jinqigufen.top/gtxmagwqew.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpacyrhao.html

[S01] C：Hello World
来源：http://hz.fzhhl.top/gtxnkprkad.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtnwipzczx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tanke756.top/gtzzsmuopg.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtmukitvwk.html

int a = 10; printf("%d\n", a);
来源：http://hz.birdmap.top/gtxyyhxoun.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtfofmuwnl.html

int x; scanf("%d", &x);
来源：http://hz.yuanzhike.top/gtuwikdmyo.html

[S04] C：字符串复制
来源：http://hz.ppjwa.cn/gtbpdrgbqp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ppjwa.cn/gtdgnqylil.html

[S05] C：字符串长度
来源：http://hz.cdnleiting.top/gtrlzkgpuz.html

strlen(s)
来源：http://hz.guowangkeji.top/gtsowceshh.html

[S06] C：字符串比较
来源：http://hz.xuetiantiany.cn/gtrblmwhlw.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gthwrmbyuj.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtyuinposr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtksgzfdvz.html

[S08] C：动态内存分配与释放
来源：http://hz.chenlongwang.top/gtojvrxdcn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtmumrwrjk.html

[S09] C：结构体定义与初始化
来源：http://hz.yonumen.top/gterltyliu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtrtgacqky.html

[S10] C：指针与解引用
来源：http://hz.yonumen.top/gtjagffmyi.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtybuyayfg.html

[S11] C：逐行读文件
来源：http://hz.havefunace.top/gtbeyqnbbz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtvwxfuwmu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cqqwz.cn/gtvzfpfwql.html

fclose(f);
来源：http://hz.yangfankeji.com/gtnfsyxwms.html

[S12] C：写文件
来源：http://hz.bjfxy.top/gtccqmiusb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtovxyrehn.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtrnaqunta.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gttnlyuvav.html

[S14] C：枚举
来源：http://hz.havefunace.top/gtsadliwmk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigufen.top/gtupbqxpmt.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtmxwbitee.html

(double) a / b
来源：http://hz.cashguo.top/gtxlshdyiu.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtusvrfalp.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gtguasdfht.html

[S17] C：安全拼接字符串
来源：http://hz.yonumen.top/gtqtphegoi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jyoumei.cn/gtgkgqnxbw.html

[S18] C：命令行参数
来源：http://hz.cashguo.top/gtjgwiblpe.html

int main(int argc, char **argv)
来源：http://hz.birdmap.top/gtpehwwwbp.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtznxffaww.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtjvqboeep.html

[S20] C：二分查找
来源：http://hz.meibo888.top/gtrzznohvy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtnpyqfgiu.html

[S21] C：字符类别判断
来源：http://hz.ydjk.org.cn/gtafuqcstt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtfrjcfisy.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gtaspbokfs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cashguo.top/gtkmuhebsj.html

[S23] C：随机数
来源：http://hz.shanyushiyangtech.top/gtcdborfsq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtelvzznka.html

[S24] C：获取本地时间
来源：http://hz.dashuyun.cn/gtkbvsksxo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtrbklqloz.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtlhyiolxo.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtrdtcepxn.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gtjhbxfoaq.html

memset(a, 0, sizeof a);
来源：http://hz.shuidangran.top/gtmhefzbez.html

[S27] C：定义常量
来源：http://hz.svipenyu.cn/gtbzvcioxs.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtfrhheyby.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtupejcfid.html

static int counter = 0;
来源：http://hz.quarkkingdee.top/gtdfvzgpdp.html

[S29] C：变参函数
来源：http://hz.mhx1999.top/gtqbhuwuov.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtxwfynitk.html

[S30] C：头文件保护
来源：http://hz.iojbl.cn/gtpayxfcgn.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtorkjvvnc.html

#define X_H
来源：http://hz.yj202588.top/gtkbylonzx.html

#endif
来源：http://hz.shanyushiyangtech.top/gtrontysoo.html

[S31] C++：Hello World
来源：http://hz.316326.xyz/gtekujlmer.html

#include <iostream>
来源：http://hz.yvedp.cn/gtinlzqczg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gtqfgykqwt.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gtnflkjzij.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtyvghmcak.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangtech.top/gtolvjpyta.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuetiantiany.cn/gtesykaxwz.html

[S34] C++：遍历 vector
来源：http://hz.xingfuxueyuan.xyz/gtshkukmqg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258.top/gtjevsmktj.html

[S35] C++：map
来源：http://hz.yj20258.top/gtogizlpnj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtwoibtpus.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtcmfbneng.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtsvbjaxdh.html

[S37] C++：set
来源：http://hz.yonumen.top/gtgkaismcv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gotoacloud.top/gtxjmvbebj.html

[S38] C++：排序
来源：http://hz.zhengqikj.top/gtnmgsxmql.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtvelhmvmx.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtdvlaeyrs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigufen.top/gtyhvminry.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtdeyrgdgn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtvfthdxtu.html

[S41] C++：类与构造函数
来源：http://hz.cashguo.top/gtcdslyqln.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.52xcode.cn/gtuudhpsbk.html

[S42] C++：继承与虚函数
来源：http://hz.hnxiangtu.top/gtzyhmmfdr.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhijiandao.cn/gtucuikuvd.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtnibwjbef.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydjk.org.cn/gtemyqtinn.html

[S44] C++：引用传参
来源：http://hz.feifeiyinyue.top/gtxapzkjqi.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtpsrvdftr.html


<!-- 参考信息 -->