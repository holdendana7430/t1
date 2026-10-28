代发 wailian999

ANALYZE TABLE users;
来源：http://hz.ehwqpu.com/gtunayfrqy.html

[Q71] 查看建表语句
来源：http://hz.havefunace.top/gtxoreuddg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuanzhike.top/gtyvkbjwlu.html

[Q72] 查看索引
来源：http://hz.gotoacloud.top/gtbqcafpxh.html

SHOW INDEX FROM users;
来源：http://hz.cashguo.top/gtdifjjqqw.html

[Q73] 查看表状态
来源：http://hz.ivvv.top/gthloizpjx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydjk.org.cn/gtunqfeawq.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtuwycgjty.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtjgtzcaqi.html

[Q75] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gtazrlhypw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuetiantiany.cn/gtkibuzuip.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtvoyotlnr.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gttrznvkje.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aibaodan.cn/gtxrrayigo.html

[Q77] 时间加减
来源：http://hz.yonumen.top/gtdwuqbwde.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtzxxghymj.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gttmghpywq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yongpay.top/gtzsxiojqr.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtylixlnbb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.52xcode.cn/gtyptuvfoo.html

[Q80] 字符串截取
来源：http://hz.yueranfly.top/gtusctmxrf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jyoumei.cn/gtkaflgyug.html

[Q81] 字符串替换
来源：http://hz.wangdashe.top/gtsfkfkzpy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gtouwimasv.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangtech.top/gtligvknel.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhoulong.xyz/gtujofjmnv.html

[Q83] 大小写转换
来源：http://hz.zycfv.cn/gtfttwjeul.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtzoncdrog.html

[Q84] 去除首尾空格
来源：http://hz.aizwys.cn/gtpindyqdq.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gtbqzxlwbx.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gtkqhvoqeu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.birdmap.top/gtgqaxwekf.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtlwdsslvm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtkdpakdrv.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtcxcdzutq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhiwuduotai.top/gtxntgqwlw.html

[Q88] 行转列（条件聚合）
来源：http://hz.316326.xyz/gtbliottil.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenjidiqi.icu/gtezrputsf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hfpthk.cn/gtdfqlpgkl.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtioxxezfx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gthrjyyvvw.html

[Q90] 生成序号列
来源：http://hz.fzhhl.top/gtpjnxfsvp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258888.top/gtethsedhv.html

================================================================================
来源：http://hz.zycfv.cn/gtfyotbiob.html

R. Bash 专题
来源：http://hz.316326.xyz/gtvfipsipa.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfzyvxjat.html

[R01] shebang 与严格模式
来源：http://hz.xuanzx.com/gtbenlvtuy.html

#!/usr/bin/env bash
来源：http://hz.guowangkeji.top/gtzbhggmrr.html

set -euo pipefail
来源：http://hz.shzxlz.cn/gtfjntzwjo.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtjzsaljbe.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtewbtcmfw.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtltfcaesl.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtzruphncn.html

[R04] 位置参数
来源：http://hz.316326.xyz/gthzgqrbej.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtaehqgapb.html

[R05] 参数默认值
来源：http://hz.ehwqpu.com/gtohyouyex.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gtwhxmcwcp.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gthcckximx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxuanxn.top/gtbxqahgaz.html

[R07] if 判断文件
来源：http://hz.xziqi.cn/gtqcxxvkkd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daxiang520.top/gtawjtmqah.html

[R08] 数值比较
来源：http://hz.tian-w.cn/gtjohwiayh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhixingplan.top/gtuyfayjns.html

[R09] 字符串比较
来源：http://hz.zhoulong.xyz/gtorhisqrk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tanke756.top/gtopwtitom.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtahzignkf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtvhlyfleu.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gttsblmgzr.html

case "$1" in
来源：http://hz.tian-w.cn/gtxuyrzfqy.html

start) echo "启动" ;;
来源：http://hz.yj20258.top/gttooatcyd.html

stop)  echo "停止" ;;
来源：http://hz.dianchejie.cn/gteosdckie.html

*)     echo "未知命令" ;;
来源：http://hz.wangdashe.top/gtjhbzdaea.html

esac
来源：http://hz.fengsongda.top/gtspeaqpgf.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtkkfllbhv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtmznbipua.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtkptcyubk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtdhmlwbhy.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtucptscww.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gthqdnpiwe.html

[R15] while 逐行读文件
来源：http://hz.yj20258888.top/gtyfztdlfu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.andypj.xyz/gtvjnhseap.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtxvjuinfz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gttyyzadwe.html

[R17] 数组定义与取值
来源：http://hz.wangshuangyany.cn/gtfthetgkg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtmnzfulzb.html

[R18] 遍历数组
来源：http://hz.aizwys.cn/gtgpuoataj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinyuanbaomall.cn/gtvxatyzmn.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtdhwdfxkd.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gtzhdetrnk.html

[R20] 关联数组（字典）
来源：http://hz.jqgfzy.top/gtztvzrrka.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigfzy.top/gtkvtnvphv.html

[R21] 字符串长度
来源：http://hz.hongshengwenyu.top/gtqdsokcqg.html

echo "${#s}"
来源：http://hz.hongshengwenyu.top/gtheldvoij.html

[R22] 截取子串
来源：http://hz.yongpay.top/gthxazdjis.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gtnvenwyij.html

[R23] 字符串替换
来源：http://hz.zycfv.cn/gtnzjvzacf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtapwwkhsw.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtdhoiqejd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shangyingyoupin.top/gtoexhxxvc.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gtddycoxlh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yangfankeji.com/gtsyrmgecc.html

[R26] 命令替换
来源：http://hz.zhiwuduotai.top/gtoqenwvjg.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtsqjwywwc.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtbhzsrjuj.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtzkjtmmmz.html

[R28] 浮点运算
来源：http://hz.yuxming.cn/gtyrejonia.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gtmzbyfmar.html

[R29] 定义函数
来源：http://hz.shuidangran.top/gtfpoxgzmv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydjk.org.cn/gtbsvgeqzf.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gtbmunfwqz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtwzlxdpyk.html

[R31] 局部变量
来源：http://hz.jinghuilouyu.cn/gtorksgjbf.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtslaekjwq.html

[R32] 参数个数校验
来源：http://hz.zycfv.cn/gtedfyfgnm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zycfv.cn/gthakztbgd.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtdupruhdi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangtech.top/gtntpaoxjh.html

[R34] 退出时清理
来源：http://hz.shangyingyoupin.top/gthbupydch.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtsmcdawov.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gttceyhilf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gtrtrozbie.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gtbdbfdpyb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hywenlv.cn/gteqfblvnx.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtgyzetkcn.html

files=$(ls -1)
来源：http://hz.hysaishi.cn/gtogkhfzyn.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtwgwuwqnn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fzhhl.top/gtwqffosnq.html

[R39] 重定向标准输出与错误
来源：http://hz.ydjk.org.cn/gtuummulqm.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtsiwiivgr.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtsvmcntrd.html

echo "log" >> out.log
来源：http://hz.zhongyouzk.top/gtkndrqlne.html

[R41] 丢弃输出
来源：http://hz.daxiang520.top/gtvmduaotv.html

cmd >/dev/null 2>&1
来源：http://hz.havefunace.top/gtwgidicda.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gtjopccpio.html

wc -l < a.txt
来源：http://hz.xylfe.cn/gtumxbkekh.html

[R43] 按名字查找文件
来源：http://hz.hnqzz.top/gtrmkiftnd.html

find . -name "*.log" -type f
来源：http://hz.jinqigfzy.top/gtmlvnvsuf.html

[R44] 按修改时间查找
来源：http://hz.zhaomingkeji.xyz/gtwyzjyyrj.html

find . -mtime -7 -type f
来源：http://hz.ivvv.top/gtzdsbtqej.html

[R45] 批量删除
来源：http://hz.gotoacloud.top/gtpqeaatlh.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtpvdgnjrw.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtjmxqlrta.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtbcjbyvro.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtyfmnqysj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.haohaochexian.top/gtqpimlioq.html

[R48] awk 取指定列
来源：http://hz.yuxming.cn/gtkaanfqsq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yanxiufei.cn/gtvaqlwoxa.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtemxtibec.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.c1oappe.top/gtumhnzxvp.html

[R50] awk 求和
来源：http://hz.nanxuanxn.top/gtdktrxzjv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenjidiqi.icu/gtaeecruzs.html

[R51] 排序去重取前几
来源：http://hz.cashguo.top/gtzzpylipg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hongshengwenyu.top/gtegoiklvo.html

[R52] 统计行数
来源：http://hz.daxiang520.top/gtprjkhsqc.html

wc -l a.txt
来源：http://hz.cashguo.top/gtutghvzez.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtvugqbnev.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtefvwjhrz.html

[R54] 比较两个文件
来源：http://hz.smart0.xyz/gtbvyihcah.html

diff a.txt b.txt
来源：http://hz.andypj.xyz/gtwomrvvmd.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtsxlawfjy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtibjtknpd.html

[R56] 远程拷贝
来源：http://hz.andypj.xyz/gtbusrspjz.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtqcsznmys.html

[R57] 远程执行命令
来源：http://hz.yj20258.top/gtdexskwjt.html

ssh user@host 'uptime'
来源：http://hz.jyoumei.cn/gtbufyekon.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gtaoaaohsm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtehewpino.html

[R59] 发 POST JSON
来源：http://hz.ehwqpu.com/gtcmhsfijm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gtndozenpp.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtijydkfqy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gtsgzaplrd.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtnbfybpac.html

df -h;  du -sh *
来源：http://hz.cucudq.cn/gtfalsbtds.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtxgzcvyga.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtxwshpspi.html

[R63] 内存与进程
来源：http://hz.mhx1999.top/gtimuxrkbf.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtcwhxlvpb.html

[R64] 结束进程
来源：http://hz.gogol.net.cn/gtjakbkovt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gtvvjtspzu.html

[R65] 查看端口占用
来源：http://hz.snrcjt.cn/gtukbrfosf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gttnuhpvya.html

[R66] 定时任务
来源：http://hz.pycfn.com/gtcbujhcqp.html

crontab -e;  crontab -l
来源：http://hz.hysaishi.cn/gtxnziqxwi.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtjiyuqogi.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtsfybddmj.html

[R68] 计算文件校验值
来源：http://hz.dashuyun.cn/gthnyzhxkd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gtwftjjcda.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtstnuytpd.html

head -c 16 /dev/urandom | base64
来源：http://hz.andypj.xyz/gtyoxljpgb.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtaxngxkce.html

date +%s;  date -d @1700000000
来源：http://hz.zhoulong.xyz/gtqlydnspr.html

[R71] 日期格式化
来源：http://hz.pycfn.com/gtxboswutn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtbgzphtim.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtfyuwvdmi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtyicidevj.html

[R73] 分割大日志
来源：http://hz.tian-w.cn/gtiqecvcxv.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtrkiscnfg.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gtiiwnojqz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhongyouzk.top/gtkhignjhr.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtiefclmrq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gtgjfdlopo.html

[R76] 使用临时文件
来源：http://hz.jqgufenzy.top/gtcrksswfs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtjmykcmdo.html

[R77] 读取用户输入
来源：http://hz.kuanghao11.cn/gtrckscmgn.html

read -rp "请输入: " ans
来源：http://hz.52xcode.cn/gtytvbqcos.html

[R78] 交互式菜单
来源：http://hz.xuanzx.com/gtvkhlbmzl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.iojbl.cn/gtlgvjktld.html

[R79] 解析命令行选项
来源：http://hz.hnxiangtu.top/gtdeijlozf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtkconivrd.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgufenzy.top/gtddjhpxkk.html

time ./run.sh
来源：http://hz.yangfankeji.com/gtveapkrhr.html

================================================================================
来源：http://hz.daria6918.cn/gtyqmlnjjm.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gtgtjnceec.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgjqjoqom.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gttnwlqozm.html

#include <stdio.h>
来源：http://hz.shuidangran.top/gtfwrrkjtk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxinkj.top/gtwqpesjdn.html

[S02] C：变量与格式化输出
来源：http://hz.gaohongyu789.top/gtttjwiyip.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtwvsxebbm.html

[S03] C：读入整数
来源：http://hz.kuanghao11.cn/gtsdspwoqt.html

int x; scanf("%d", &x);
来源：http://hz.c1oappe.top/gtscetqkzz.html

[S04] C：字符串复制
来源：http://hz.zhoulong.xyz/gtaeyezhce.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gtcuxkikha.html

[S05] C：字符串长度
来源：http://hz.nwbrower.top/gtuvygqebh.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtieyhfzzy.html

[S06] C：字符串比较
来源：http://hz.hywenlv.cn/gtuududhnh.html

strcmp(a, b) == 0
来源：http://hz.daria6918.cn/gtaayfgasx.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtmsexttlj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhijiandao.cn/gtuxbnfaol.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtikwzvhny.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gthmntgifv.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtjgizwcwf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gtckxtqnsd.html

[S10] C：指针与解引用
来源：http://hz.ppjwa.cn/gttvaqwupy.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtfsjtaihd.html

[S11] C：逐行读文件
来源：http://hz.quarkkingdee.top/gtpgcdfuus.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jlsjyb.cn/gtxpfxbkki.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigfzy.top/gtqnihonis.html

fclose(f);
来源：http://hz.shzxlz.cn/gtikrduzmf.html

[S12] C：写文件
来源：http://hz.hammf.cn/gtltvdrerv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guowangkeji.top/gtgiuojyso.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtrfdvkgkh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtlgydsqha.html

[S14] C：枚举
来源：http://hz.gogol.net.cn/gtlofoptdo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtrglmpqkm.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtzpenjygv.html

(double) a / b
来源：http://hz.cqqwz.cn/gtjyvmgsna.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gtwwcaddll.html

x |= (1 << 3);
来源：http://hz.pengpengdd.cyou/gttsfmferp.html

[S17] C：安全拼接字符串
来源：http://hz.bjfxy.top/gtnnfrrabg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.quarkkingdee.top/gtiginlnec.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gtivapbqfn.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtmidlpsla.html

[S19] C：快速排序
来源：http://hz.andypj.xyz/gtrxmtxiua.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtjmfevqpz.html

[S20] C：二分查找
来源：http://hz.havefunace.top/gtxqtcwbtk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtmifzqsmp.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtghsdocdy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhiwuduotai.top/gtwspyqkxd.html

[S22] C：字符串转数字
来源：http://hz.hnqzz.top/gternwpfyc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pengpengdd.cyou/gtybazwsnj.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtvkisqwhs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gttfhksobo.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtsfqyrzyw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtvjecowge.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gtbezfuaaz.html

memcpy(dst, src, n);
来源：http://hz.pengpengdd.cyou/gtxhcyfkti.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtjvrhukkj.html

memset(a, 0, sizeof a);
来源：http://hz.vqdsnc.cn/gtijlmkxmu.html

[S27] C：定义常量
来源：http://hz.nanxinkj.top/gtqpsngrkb.html

const double PI = 3.14159;
来源：http://hz.birdmap.top/gthjgrmbdf.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtqeppqlrh.html

static int counter = 0;
来源：http://hz.shuidangran.top/gtfscyoqbc.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gtemwqfiwl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtcdmovjeh.html

[S30] C：头文件保护
来源：http://hz.cucudq.cn/gtwmiouunl.html

#ifndef X_H
来源：http://hz.kuanghao11.cn/gtmakyooen.html

#define X_H
来源：http://hz.zycfv.cn/gtetwgrjuu.html

#endif
来源：http://hz.xylfe.cn/gtbjdohhjb.html

[S31] C++：Hello World
来源：http://hz.jianghu66.top/gtdsezriws.html

#include <iostream>
来源：http://hz.quarkkingdee.top/gtwnfnfacc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtujdgevvy.html

[S32] C++：字符串
来源：http://hz.jianghu66.top/gthxdjfztp.html

std::string s = "hi";  s += "!";
来源：http://hz.haohaochexian.top/gttxtgcdam.html

[S33] C++：vector 增删
来源：http://hz.sysykeji.top/gtetmpizym.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtallxduft.html

[S34] C++：遍历 vector
来源：http://hz.cdnleiting.top/gtehxffxat.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gtbhmplyjn.html

[S35] C++：map
来源：http://hz.gzhubu.top/gthrtdvids.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtbsxpreth.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtndruosyh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtmxnxndrb.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtbpsemibf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtxrmlsaxc.html

[S38] C++：排序
来源：http://hz.yvedp.cn/gtufboaimi.html

std::sort(v.begin(), v.end());
来源：http://hz.hysaishi.cn/gtkuymlzah.html

[S39] C++：自定义比较器排序
来源：http://hz.yongpay.top/gtqcfnovlt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sxryk.cn/gtlvzhmexf.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gttfrbyvnk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtkdhyvwzh.html


<!-- 参考信息 -->