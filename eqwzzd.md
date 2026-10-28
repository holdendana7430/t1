代发 wailian999

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtvitoctsr.html

[Q71] 查看建表语句
来源：http://hz.mhx1999.top/gtxvamydhj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gtcmznizpx.html

[Q72] 查看索引
来源：http://hz.52xcode.cn/gtzjxjdcfg.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtsfytbrrk.html

[Q73] 查看表状态
来源：http://hz.jlsjyb.cn/gtipafscfr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtqptsxmum.html

[Q74] 强制使用索引
来源：http://hz.daxiang520.top/gthlerodig.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shangyingyoupin.top/gtdzanetks.html

[Q75] 日期格式化
来源：http://hz.snrcjt.cn/gttgxcqtbg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.redwolf501.top/gtupkztegp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tanke756.top/gtefqntanm.html

[Q76] 按天统计
来源：http://hz.ppjwa.cn/gtptuvgdjg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ybcxt.top/gtfenapbjm.html

[Q77] 时间加减
来源：http://hz.0kj1m.cn/gtdvzqruox.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtjbrzsdpi.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtecckzbyd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtjnfipxaj.html

[Q79] 字符串拼接
来源：http://hz.zdqjudy.top/gtcneflfgg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtvlcjvsda.html

[Q80] 字符串截取
来源：http://hz.quarkkingdee.top/gtkygtterw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtqpcyejjv.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtskebywxs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtmsdxznwd.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gttvtsktsg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgufenzy.top/gtorijenez.html

[Q83] 大小写转换
来源：http://hz.cashguo.top/gtdlkjxsyh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sysykeji.top/gtoztthqyi.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtpwosceqv.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gtlrmifbqi.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gthcrkooaz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtsphogegb.html

[Q86] 读取 JSON 字段
来源：http://hz.yanxiufei.cn/gtmpudfrqb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangkeji.top/gtlfuxmjtz.html

[Q87] JSON 字段做条件
来源：http://hz.havefunace.top/gthxcrckcg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shzxlz.cn/gtsvnkkbmy.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtyixgazng.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gtjmppjfjv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtlvvtqwnh.html

[Q89] 判断表是否存在
来源：http://hz.sweek.top/gtpmtshhpx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gteeoonroz.html

[Q90] 生成序号列
来源：http://hz.tianlin.xyz/gtswhnuzrj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258.top/gtfqmudqjw.html

================================================================================
来源：http://hz.0kj1m.cn/gtpuuteyaz.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtyxrjwrfj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtyixftzqy.html

[R01] shebang 与严格模式
来源：http://hz.yj20258.top/gthpmooprf.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtmddimyip.html

set -euo pipefail
来源：http://hz.tanke756.top/gtkbksrqxi.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtzcxkyaus.html

name="Tom"; echo "$name"
来源：http://hz.andypj.xyz/gtkzicgxoa.html

[R03] 只读变量
来源：http://hz.hfpthk.cn/gtrhgufknq.html

readonly PI=3.14
来源：http://hz.yj202588.top/gtbukmhtzw.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtfqboxjzi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtvvdfqrie.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtvwejdksy.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gtjiozphfc.html

[R06] 判断命令是否存在
来源：http://hz.quarkkingdee.top/gtfdykikbw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtbsfrabmk.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtrllojqsm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gtbamzsjom.html

[R08] 数值比较
来源：http://hz.jqgfzy.top/gtqikgswed.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangdashe.top/gteqwdefjm.html

[R09] 字符串比较
来源：http://hz.cdnleiting.top/gtfffkkmzg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.c1oappe.top/gtlvxmrbss.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtqidrzghy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gtmboylyal.html

[R11] case 多分支
来源：http://hz.shuidangran.top/gtzxwwroee.html

case "$1" in
来源：http://hz.xylfe.cn/gtyqeorjdw.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gtcodwckbi.html

stop)  echo "停止" ;;
来源：http://hz.bjfxy.top/gtlzaxfhqb.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtyqkjqpjf.html

esac
来源：http://hz.jqgufenzy.top/gtjeofkjgv.html

[R12] for 遍历文件
来源：http://hz.aizwys.cn/gticmomnqt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtltbhimmh.html

[R13] for 计数循环
来源：http://hz.havefunace.top/gtnxgvtxqj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhengqikj.top/gtdcttgvva.html

[R14] C 风格 for
来源：http://hz.jianghu66.top/gtfjmvdqqo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.birdmap.top/gtbfiexsyh.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtovwclkqh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtvgejpbqw.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gtengmwufn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gzhubu.top/gtfhfcytvw.html

[R17] 数组定义与取值
来源：http://hz.jinghuilouyu.cn/gtgxohstsr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtyaetmkdh.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gthkobmjzk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtxlepdrtt.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtlwgkoibz.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtshawqhpy.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gtyfwtkqkk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtzpqvwjmo.html

[R21] 字符串长度
来源：http://hz.feifeiyinyue.top/gtowhdgzjh.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtdygauuen.html

[R22] 截取子串
来源：http://hz.jlsjyb.cn/gtkpnaelan.html

echo "${s:0:5}"
来源：http://hz.yj20258888.top/gtidzwuvni.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gttghhedoc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.havefunace.top/gtwigrblcx.html

[R24] 大小写转换
来源：http://hz.cashguo.top/gtbpheclvz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gtacedaudi.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinyuanbaomall.cn/gtaxwexfig.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.svipenyu.cn/gtubyhnmoa.html

[R26] 命令替换
来源：http://hz.daxiang520.top/gtxycvstgj.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gthziakbvz.html

[R27] 算术展开
来源：http://hz.haohaochexian.top/gtmjveuhpj.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtmmbkkcot.html

[R28] 浮点运算
来源：http://hz.hnqzz.top/gthltkxqge.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtynlykdzc.html

[R29] 定义函数
来源：http://hz.andypj.xyz/gtxgpldoxw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yvedp.cn/gtqtlclqwt.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtxrfvzlrg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtpzltotus.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtnqbisqep.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258.top/gtflyozzgf.html

[R32] 参数个数校验
来源：http://hz.tianlin.xyz/gtwdydjywi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtivhkrwfq.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gtcnaaynrd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xingfuxueyuan.xyz/gttympgoym.html

[R34] 退出时清理
来源：http://hz.fengsongda.top/gtqxxpluvj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtscyzbfml.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtjdzdlydm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tian-w.cn/gtezdlckwb.html

[R36] 并发执行多个任务
来源：http://hz.9152youxi.cn/gtzgvzhhpt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nwbrower.top/gtwhuwazib.html

[R37] 把输出赋给变量
来源：http://hz.yonumen.top/gtjwsemkhi.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtsdrtzbyi.html

[R38] 管道串联
来源：http://hz.yvedp.cn/gtqumtwgps.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangdashe.top/gtejukhbfh.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtkrenjhdw.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtnfacfgms.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtfkhqfkuy.html

echo "log" >> out.log
来源：http://hz.hnqzz.top/gtktfutflf.html

[R41] 丢弃输出
来源：http://hz.haohaochexian.top/gtugqwzdao.html

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtvrrfvkxz.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtaralufih.html

wc -l < a.txt
来源：http://hz.birdmap.top/gtixpcdzsp.html

[R43] 按名字查找文件
来源：http://hz.guowangkeji.top/gttzbetnfx.html

find . -name "*.log" -type f
来源：http://hz.havefunace.top/gtuuzqeouw.html

[R44] 按修改时间查找
来源：http://hz.ybcxt.top/gtbvatauwh.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtbinewjzk.html

[R45] 批量删除
来源：http://hz.52xcode.cn/gtvhwgxrkk.html

find . -name "*.tmp" -delete
来源：http://hz.zhongyouzk.top/gtowkbgmes.html

[R46] 递归替换文件内容
来源：http://hz.zhixingplan.top/gtrvouxvxz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zdqjudy.top/gtaoibwqci.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gteqgtwycf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hywenlv.cn/gtvzapnlmi.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gttiphcegu.html

awk '{print $1, $3}' a.txt
来源：http://hz.jiagoushi.top/gtwfymuktb.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gtgduoizgl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shzxlz.cn/gtilossxnb.html

[R50] awk 求和
来源：http://hz.andypj.xyz/gtprxliqwx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtuoepvquq.html

[R51] 排序去重取前几
来源：http://hz.quarkkingdee.top/gtorcwoawn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtfgfwizvc.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtyqlhomux.html

wc -l a.txt
来源：http://hz.tianlin.xyz/gtyfopooyn.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtnqdnlhag.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fengsongda.top/gtbebddmaj.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gttacqocne.html

diff a.txt b.txt
来源：http://hz.feifeiyinyue.top/gtklnvsdhh.html

[R55] 压缩与解压
来源：http://hz.ivvv.top/gtnqvkfcey.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtbyegkulq.html

[R56] 远程拷贝
来源：http://hz.chenlongwang.top/gtmxcjkonm.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtscgoqcgf.html

[R57] 远程执行命令
来源：http://hz.hnqzz.top/gtrtfccsja.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtocqovqvr.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtivarniem.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cheryme.top/gtlvbmokry.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gtqolpjpkf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtofxqrhgh.html

[R60] 只看 HTTP 状态码
来源：http://hz.daria6918.cn/gtmcpjfmtz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gtqxmugzeg.html

[R61] 磁盘占用
来源：http://hz.sweek.top/gtaxojwypl.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gtausfmbip.html

[R62] 找最占空间的文件
来源：http://hz.guowangkeji.top/gtshjbtfls.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtempmokbo.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gtdfueexqv.html

free -h;  ps aux | grep nginx
来源：http://hz.dianchejie.cn/gtzkxxruif.html

[R64] 结束进程
来源：http://hz.snrcjt.cn/gtqhtbsxfo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.52xcode.cn/gtuoszwhrw.html

[R65] 查看端口占用
来源：http://hz.jlsjyb.cn/gtptkmtqzg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fzhhl.top/gtwwviwnxa.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtzrengdmw.html

crontab -e;  crontab -l
来源：http://hz.yangfankeji.com/gtyxebrnpq.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtdrdfammo.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtfsmfynik.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtoazbxovj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtisbszbzd.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtwthjimwf.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtvufzsrnw.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtbydicxqn.html

date +%s;  date -d @1700000000
来源：http://hz.pengpengdd.cyou/gtqdkeuaxr.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gthuvhysha.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtsrytcqcd.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangtech.top/gtkrywiwzh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenzaomai.com/gtjnnbjadr.html

[R73] 分割大日志
来源：http://hz.wangshuangyany.cn/gtffvkznuw.html

split -l 1000 big.log part_
来源：http://hz.fzhhl.top/gtkyidlris.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtmsdxtmsk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhongyouzk.top/gtzywvsycf.html

[R75] 导出环境变量
来源：http://hz.yongpay.top/gtvtdnxkbx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtnfibgjja.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtuvotuubh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtxtvvehrp.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtimkzdukg.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangkeji.top/gtgopgzqie.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtklsaxhsr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daxiang520.top/gtvigypjdz.html

[R79] 解析命令行选项
来源：http://hz.cdnleiting.top/gtrphblnyr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pycfn.com/gtirboyjhg.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtadzxgwjl.html

time ./run.sh
来源：http://hz.gzhubu.top/gtiycsyjsn.html

================================================================================
来源：http://hz.cdnleiting.top/gtlkrtjfcq.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gtakblioiq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwtfdolmu.html

[S01] C：Hello World
来源：http://hz.zhixingplan.top/gtqlkdplin.html

#include <stdio.h>
来源：http://hz.hnqzz.top/gtprivueos.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtqosowgop.html

[S02] C：变量与格式化输出
来源：http://hz.svipenyu.cn/gtpxxssvhb.html

int a = 10; printf("%d\n", a);
来源：http://hz.cqqwz.cn/gtmhyzvrjz.html

[S03] C：读入整数
来源：http://hz.hnqzz.top/gtxjamchqh.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtqiesnbip.html

[S04] C：字符串复制
来源：http://hz.meibo888.top/gtopvjzkrd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jlsjyb.cn/gtlgqqigli.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtmmoxdqgw.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gttndkzaoc.html

[S06] C：字符串比较
来源：http://hz.quarkkingdee.top/gtdjfsvuya.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gticpqvcic.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtwnnxwkfh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gttjneaftr.html

[S08] C：动态内存分配与释放
来源：http://hz.wangdashe.top/gtqcgrxppi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.smart0.xyz/gtnyftnqgg.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gtifdltczk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cdnleiting.top/gthmqdrbnp.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtxysakdyr.html

int *p = &a;  *p = 5;
来源：http://hz.vqdsnc.cn/gtwrntvesn.html

[S11] C：逐行读文件
来源：http://hz.haohaochexian.top/gtvrnrpagn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gteqlckjjr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnxiangtu.top/gttyfpivmu.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtnjzfcllr.html

[S12] C：写文件
来源：http://hz.hammf.cn/gthsmmzyzk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gogol.net.cn/gtwizlhcxc.html

[S13] C：宏定义
来源：http://hz.yonumen.top/gtcvssljby.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hywenlv.cn/gtfisylsla.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtfvxwslpo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.haohaochexian.top/gttyyxhbcx.html

[S15] C：类型转换
来源：http://hz.pycfn.com/gtxjisxhby.html

(double) a / b
来源：http://hz.yongpay.top/gtwvpkyuri.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gttbgelimk.html

x |= (1 << 3);
来源：http://hz.c1oappe.top/gtmunbhudf.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gtcxlwdvus.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.guowangkeji.top/gtonhemrhc.html

[S18] C：命令行参数
来源：http://hz.aizwys.cn/gtbbejfmgk.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gttknkeemq.html

[S19] C：快速排序
来源：http://hz.fengsongda.top/gteoxywcli.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtsflpqsxe.html

[S20] C：二分查找
来源：http://hz.sweek.top/gtdycwvcup.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtutybqyou.html

[S21] C：字符类别判断
来源：http://hz.guannengcc.top/gtynocahur.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gthwjxsleb.html

[S22] C：字符串转数字
来源：http://hz.yuxming.cn/gtjrrpxktm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.bjfxy.top/gtxbzhrobd.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtgzrwhocd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtckzmpcjt.html

[S24] C：获取本地时间
来源：http://hz.xziqi.cn/gtpzigmayv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.havefunace.top/gttorsenap.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtkeuwadrh.html

memcpy(dst, src, n);
来源：http://hz.dashuyun.cn/gthflgzkpx.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtaubgbkqw.html

memset(a, 0, sizeof a);
来源：http://hz.zhijiandao.cn/gttyzlbhuz.html

[S27] C：定义常量
来源：http://hz.feifeiyinyue.top/gtpzoqrduf.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtzzhwysom.html

[S28] C：静态变量
来源：http://hz.316326.xyz/gtsnbusjbs.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gteknknbwk.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtbddccqow.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinyuanbaomall.cn/gtoukvksoe.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangtech.top/gtubyzjjsj.html

#ifndef X_H
来源：http://hz.hammf.cn/gtxoerozrh.html

#define X_H
来源：http://hz.hnqzz.top/gtlubmiryo.html

#endif
来源：http://hz.haohaochexian.top/gtfscjhrta.html

[S31] C++：Hello World
来源：http://hz.feifeiyinyue.top/gtnyfnkqwe.html

#include <iostream>
来源：http://hz.hnqzz.top/gtbiobloxc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hfpthk.cn/gtqyvtckjj.html

[S32] C++：字符串
来源：http://hz.cheryme.top/gteyaxrmkc.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258888.top/gtgdfovmsm.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gtsvqrepxv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fzhhl.top/gtuudlpjbi.html

[S34] C++：遍历 vector
来源：http://hz.nanxinkj.top/gtiehiglru.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinyuanbaomall.cn/gtoyvprlui.html

[S35] C++：map
来源：http://hz.daxiang520.top/gtxdhjpvoe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtxwavgnho.html

[S36] C++：unordered_map
来源：http://hz.yanxiufei.cn/gtdvpolnnh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtbsfqdrqr.html

[S37] C++：set
来源：http://hz.52xcode.cn/gtkasfensx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtwspqxsdu.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtvmqnfyza.html

std::sort(v.begin(), v.end());
来源：http://hz.jiagoushi.top/gthggdbpub.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtwniocmbw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuxming.cn/gtztvsottq.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtusezpiyd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtpvuvozxj.html


<!-- 参考信息 -->