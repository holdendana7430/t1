代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.yj20258.top/gtoqyadbdy.html

[Q73] 查看表状态
来源：http://hz.shangyingyoupin.top/gtxivdwuts.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtcddpgdid.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtzinhumno.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtqkyodxoh.html

[Q75] 日期格式化
来源：http://hz.ywan-chungtsiang.top/gtifhohyms.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtcrooslsh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gttekxrnfa.html

[Q76] 按天统计
来源：http://hz.yangfankeji.com/gtadwuyyhs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hammf.cn/gthwlxuvqt.html

[Q77] 时间加减
来源：http://hz.redwolf501.top/gttmiamyrd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tanke756.top/gthjygbriq.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gthwfqyfwp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fengsongda.top/gtljjvoicd.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtgzahhckr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.quarkkingdee.top/gtittplhba.html

[Q80] 字符串截取
来源：http://hz.havefunace.top/gtfealyhuq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daxiang520.top/gtbtiluoed.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtkoikcyet.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.smart0.xyz/gthmvwpxww.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtckeqqklz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhijiandao.cn/gthwwnqdnp.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtcpyeypwj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtflgedxir.html

[Q84] 去除首尾空格
来源：http://hz.zhiwuduotai.top/gtijggmhvl.html

SELECT TRIM(name) FROM users;
来源：http://hz.aizwys.cn/gtpbouyqob.html

[Q85] 数值取整
来源：http://hz.c1oappe.top/gtvukwahax.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.andypj.xyz/gtiwohntrm.html

[Q86] 读取 JSON 字段
来源：http://hz.tanke756.top/gtbqowepkc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gaohongyu789.top/gtvgmuktaj.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtdhpticob.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtwgwjkasv.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangtech.top/gtqzuwsmey.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gtykdwissk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ppjwa.cn/gtyeyxscoh.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gtlbryuovn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtetgujxqp.html

[Q90] 生成序号列
来源：http://hz.chenjidiqi.icu/gtndehyhcc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtvoszkaju.html

================================================================================
来源：http://hz.c1oappe.top/gtdfmpvouo.html

R. Bash 专题
来源：http://hz.yvedp.cn/gtigequzqe.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjgmppqio.html

[R01] shebang 与严格模式
来源：http://hz.yj20258.top/gtuflotceo.html

#!/usr/bin/env bash
来源：http://hz.xylfe.cn/gtofxjbbek.html

set -euo pipefail
来源：http://hz.ivvv.top/gtqiicgdxc.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtcwuddsds.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtnzskfman.html

[R03] 只读变量
来源：http://hz.52xcode.cn/gtuzbhwbcs.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtzfxyvlta.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gtdfhyyxur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenjidiqi.icu/gtkwkjevov.html

[R05] 参数默认值
来源：http://hz.jianghu66.top/gtfdmrblge.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtykflyndx.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtwkdvssan.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtzcputjib.html

[R07] if 判断文件
来源：http://hz.jlsjyb.cn/gtxgttysfw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cheryme.top/gtcsnlebcn.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtkddzvdki.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.svipenyu.cn/gttoktpejx.html

[R09] 字符串比较
来源：http://hz.sxryk.cn/gtujwchers.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sweek.top/gtfalqoapt.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtokyyppuu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtmrcqfosn.html

[R11] case 多分支
来源：http://hz.jyoumei.cn/gtfvvytgri.html

case "$1" in
来源：http://hz.9152youxi.cn/gtrmzfjevb.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gtximelezf.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtcpztcmhi.html

*)     echo "未知命令" ;;
来源：http://hz.zdqjudy.top/gtfunwxgql.html

esac
来源：http://hz.ybcxt.top/gtexzuczfd.html

[R12] for 遍历文件
来源：http://hz.cqqwz.cn/gtgqxpcgeo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.quarkkingdee.top/gtsdahpkfd.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gtwxnexfjh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gzhubu.top/gtujtwkcjw.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtbiwnufae.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tanke756.top/gtxxrakoei.html

[R15] while 逐行读文件
来源：http://hz.nwbrower.top/gtnfqezoxb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ywan-chungtsiang.top/gtmihaspul.html

[R16] until 等待条件
来源：http://hz.chenzaomai.com/gtturslfbr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ybcxt.top/gtxbdqttzq.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtdnieforf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tian-w.cn/gtxzxuumod.html

[R18] 遍历数组
来源：http://hz.gogol.net.cn/gtrxddsnxe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtmqcpmnhk.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gthjktwvzv.html

echo "${#arr[@]}"
来源：http://hz.pycfn.com/gtnvlntvil.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangkeji.top/gtcpgbyezt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtwijjnyym.html

[R21] 字符串长度
来源：http://hz.andypj.xyz/gtghwxglsz.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtoiwxpxqa.html

[R22] 截取子串
来源：http://hz.dashuyun.cn/gtuvxvemeq.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtciitsayy.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtmgvhsyio.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haohaochexian.top/gtalvmemkj.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtcgrvzfrf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgufenzy.top/gtmdurvywe.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtwlikilwa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gtxsgzlssd.html

[R26] 命令替换
来源：http://hz.chenzaomai.com/gtvspkrkup.html

now=$(date +%F); echo "$now"
来源：http://hz.hfpthk.cn/gtfjioimkf.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtwfqcpjvx.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtehzuofyj.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtwqvprfhk.html

echo "scale=2; 10/3" | bc
来源：http://hz.hywenlv.cn/gtgvyxsgxn.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtzmvnmfqr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gthkvluilr.html

[R30] 函数返回状态码
来源：http://hz.xylfe.cn/gtfujgaokk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ywan-chungtsiang.top/gtvyxrhrnn.html

[R31] 局部变量
来源：http://hz.fengsongda.top/gtfpzdwbbz.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gttqpkfhut.html

[R32] 参数个数校验
来源：http://hz.iojbl.cn/gtkgklherr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtandkljwm.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtzhaqrved.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xinyue.icu/gtyvcdvmvn.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtilnelbgu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtxxmysmfx.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gthcicuzcb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gzhubu.top/gtyverqmbr.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtfjidbuam.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jlsjyb.cn/gtnklbddyi.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gthtxruqmj.html

files=$(ls -1)
来源：http://hz.xziqi.cn/gtnhslmtjz.html

[R38] 管道串联
来源：http://hz.ppjwa.cn/gtauymyujv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtpkbkeqrh.html

[R39] 重定向标准输出与错误
来源：http://hz.aizwys.cn/gtekdhfoln.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtgyxnrzmc.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtzmylaalk.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtespyqhwp.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtzhozitgy.html

cmd >/dev/null 2>&1
来源：http://hz.hfpthk.cn/gtxsqttlrl.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtkbjstlvb.html

wc -l < a.txt
来源：http://hz.hammf.cn/gtkmwbqrdg.html

[R43] 按名字查找文件
来源：http://hz.jlsjyb.cn/gtuthszrig.html

find . -name "*.log" -type f
来源：http://hz.tianlin.xyz/gtktqnyvxs.html

[R44] 按修改时间查找
来源：http://hz.xuetiantiany.cn/gtvooxwixq.html

find . -mtime -7 -type f
来源：http://hz.hysaishi.cn/gthwgbaweg.html

[R45] 批量删除
来源：http://hz.hammf.cn/gtppsznnam.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtxqdkxogd.html

[R46] 递归替换文件内容
来源：http://hz.yj20258.top/gtgbgkdrpu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.quarkkingdee.top/gthhwpftwu.html

[R47] sed 单行替换
来源：http://hz.yuxming.cn/gtwarvryen.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daxiang520.top/gtsfaawmuw.html

[R48] awk 取指定列
来源：http://hz.birdmap.top/gtuaisdlvs.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtkchfxfup.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtadklsaud.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hongshengwenyu.top/gttaevzohb.html

[R50] awk 求和
来源：http://hz.vqdsnc.cn/gtdfgvlqil.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.vqdsnc.cn/gttppyszeo.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtukzafzek.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gtkinddyar.html

[R52] 统计行数
来源：http://hz.yj20258.top/gthoeisgbf.html

wc -l a.txt
来源：http://hz.fzhhl.top/gttjjlqaxp.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gttrkrfbcp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtfaklgblw.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtrsyvktcp.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtdiditdyh.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtjrkknamm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jianghu66.top/gtnesymxhk.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtkhbkvdyt.html

scp file user@host:/path/
来源：http://hz.xylfe.cn/gtmywtmoui.html

[R57] 远程执行命令
来源：http://hz.fzhhl.top/gtfgnbgztf.html

ssh user@host 'uptime'
来源：http://hz.jlsjyb.cn/gtjhmdgufl.html

[R58] 下载文件
来源：http://hz.zhixingplan.top/gtfjhmadyq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gtoclsjrqt.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gtnoycuhfv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.svipenyu.cn/gtpxjmxbxm.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtsghbuiap.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guowangkeji.top/gtuympkjyc.html

[R61] 磁盘占用
来源：http://hz.wangdashe.top/gtqtyficzx.html

df -h;  du -sh *
来源：http://hz.sweek.top/gtzkuwysew.html

[R62] 找最占空间的文件
来源：http://hz.hnqzz.top/gtvadpgpjo.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangkeji.top/gtmsqmqjgd.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtocombggx.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gttfrdoxmy.html

[R64] 结束进程
来源：http://hz.feifeiyinyue.top/gtahyhpyme.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgfzy.top/gtegwuitxi.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtzftbvlxm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hysaishi.cn/gtrposnupx.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtrusomxgh.html

crontab -e;  crontab -l
来源：http://hz.redwolf501.top/gtwggocfhs.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtselimuuo.html

openssl rand -hex 16
来源：http://hz.zhoulong.xyz/gtoeuyjyvg.html

[R68] 计算文件校验值
来源：http://hz.sweek.top/gtfjvfrnys.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yueranfly.top/gtcdqqkatk.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtnvaliqhx.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtnrroxngd.html

[R70] 时间戳与互转
来源：http://hz.ydzc1.top/gtsccsyfiv.html

date +%s;  date -d @1700000000
来源：http://hz.zhixingplan.top/gtgfvruwaw.html

[R71] 日期格式化
来源：http://hz.zhengqikj.top/gtpynrolls.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zycfv.cn/gtqdfjczhm.html

[R72] 等待端口就绪
来源：http://hz.zhijiandao.cn/gtkzzhxpzt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ybcxt.top/gtabodxisx.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gtfumruryl.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gtvuetkstn.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtachczbem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.mhx1999.top/gtihixyjta.html

[R75] 导出环境变量
来源：http://hz.cqqwz.cn/gtjdfwzzhj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.vqdsnc.cn/gtmtvybsrr.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtsvhivksh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtykhvdylg.html

[R77] 读取用户输入
来源：http://hz.jyoumei.cn/gtbpobeqvj.html

read -rp "请输入: " ans
来源：http://hz.andypj.xyz/gtyysvbjru.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtrotszkpy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangkeji.top/gttptkkzaa.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtvaapondw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtmppkaikt.html

[R80] 查看脚本执行耗时
来源：http://hz.hnxiangtu.top/gtyelfmrwk.html

time ./run.sh
来源：http://hz.tian-w.cn/gticrqpytd.html

================================================================================
来源：http://hz.tian-w.cn/gtyaioygwi.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtphjthxlq.html

================================================================================
来源：http://hz.yuanzhike.top/gtmpmpjfug.html

[S01] C：Hello World
来源：http://hz.ivvv.top/gtnyelfdvu.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gtbxdqpvld.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pengpengdd.cyou/gtksdzvkkr.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gtfvtvatmi.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhixingplan.top/gthbiytlcw.html

[S03] C：读入整数
来源：http://hz.yongpay.top/gtacknnofp.html

int x; scanf("%d", &x);
来源：http://hz.wangdashe.top/gtnwfyrkjz.html

[S04] C：字符串复制
来源：http://hz.hywenlv.cn/gtnisfcxyn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtmzctfzxn.html

[S05] C：字符串长度
来源：http://hz.yj20258.top/gtuuebhwzl.html

strlen(s)
来源：http://hz.nanxuanxn.top/gtazdcsgxs.html

[S06] C：字符串比较
来源：http://hz.wangshuangyany.cn/gtrdmhjnjm.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtepwwcmli.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gtfpvvnknr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.smart0.xyz/gttqkmohnd.html

[S08] C：动态内存分配与释放
来源：http://hz.mhx1999.top/gtggkxhqcp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gogol.net.cn/gtlmiutoli.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtkvyajfpu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cashguo.top/gtgdlfkrju.html

[S10] C：指针与解引用
来源：http://hz.shangyingyoupin.top/gtemoghfeu.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtduegmmwb.html

[S11] C：逐行读文件
来源：http://hz.zycfv.cn/gtwldmpgwy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daxiang520.top/gtystzucms.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yongpay.top/gtxqmpsnbu.html

fclose(f);
来源：http://hz.cheryme.top/gtcylmvqvz.html

[S12] C：写文件
来源：http://hz.sxryk.cn/gtalcgekoc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangshuangyany.cn/gtwflnxtpp.html

[S13] C：宏定义
来源：http://hz.haohaochexian.top/gtkwjgmccg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigufen.top/gtqfhyvloy.html

[S14] C：枚举
来源：http://hz.nwbrower.top/gtkfjfqlsp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtezlsbjra.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtbpsdnpku.html

(double) a / b
来源：http://hz.xinyue.icu/gttrprdhgh.html

[S16] C：位操作置位
来源：http://hz.c1oappe.top/gtikxqtsbg.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtqkcmmxye.html

[S17] C：安全拼接字符串
来源：http://hz.shuidangran.top/gtqyppfspz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dashuyun.cn/gtypnayyxy.html

[S18] C：命令行参数
来源：http://hz.aibaodan.cn/gtqkcqkjeg.html

int main(int argc, char **argv)
来源：http://hz.hfpthk.cn/gtixhcnymd.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtnolojxfx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gttlhflhhb.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gthyoimhnz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtgtpkuonk.html

[S21] C：字符类别判断
来源：http://hz.xingfuxueyuan.xyz/gtjqesgwsj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtbbdlogmi.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gtrpjyuzyg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.quarkkingdee.top/gttwyqjwcd.html

[S23] C：随机数
来源：http://hz.shangyingyoupin.top/gtyjzfjkvv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ppjwa.cn/gtmxvhaqeq.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtpqvtjqka.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gtnivqapzo.html

[S25] C：内存拷贝
来源：http://hz.birdmap.top/gtbkdxdelz.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gtbnrqhmff.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtmiaqdadj.html

memset(a, 0, sizeof a);
来源：http://hz.yongpay.top/gtctmqubik.html

[S27] C：定义常量
来源：http://hz.aibaodan.cn/gtiajophoe.html

const double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtwtcinynj.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gttkrrcpmm.html

static int counter = 0;
来源：http://hz.shuidangran.top/gtolohzmbb.html

[S29] C：变参函数
来源：http://hz.daria6918.cn/gtlakjvhft.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yangfankeji.com/gtwsjbrtqq.html

[S30] C：头文件保护
来源：http://hz.bjfxy.top/gtzqgvmujf.html

#ifndef X_H
来源：http://hz.jinqigufen.top/gtdwqrofvd.html

#define X_H
来源：http://hz.shangyingyoupin.top/gtkvkhvfjb.html

#endif
来源：http://hz.gaohongyu789.top/gtlvfrokzi.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtrtanjphn.html

#include <iostream>
来源：http://hz.hywenlv.cn/gtxnnqmfzh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtaygesfwb.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtqtxuuhnb.html

std::string s = "hi";  s += "!";
来源：http://hz.vqdsnc.cn/gtqlmxtnbf.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangtech.top/gtmbnyvgdf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gthjhfnain.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gttejdebia.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenzaomai.com/gtkqeavkfa.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtjfmsrmgu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtazbekupc.html

[S36] C++：unordered_map
来源：http://hz.gogol.net.cn/gtokzclvcx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtytvdhxwt.html

[S37] C++：set
来源：http://hz.gogol.net.cn/gtjdgtviuv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gttaoacmwm.html

[S38] C++：排序
来源：http://hz.ivvv.top/gtcraomlnz.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtowvnunsd.html

[S39] C++：自定义比较器排序
来源：http://hz.quarkkingdee.top/gtooofibrl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtjmilzeqv.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gtjmpxocpr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yanxiufei.cn/gtzrefqzie.html

[S41] C++：类与构造函数
来源：http://hz.jlsjyb.cn/gtyerpwnnf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tianlin.xyz/gtysyztdmx.html

[S42] C++：继承与虚函数
来源：http://hz.jinghuilouyu.cn/gtvquifbpn.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtbexfmmac.html


<!-- 参考信息 -->