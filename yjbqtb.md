代发 wailian999

[Q63] 开启事务
来源：http://hz.wangshuangyany.cn/gtrdnalqvn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daxiang520.top/gtxehxoyqy.html

[Q64] 提交事务
来源：http://hz.gotoacloud.top/gtnigacywi.html

COMMIT;
来源：http://hz.chenzaomai.com/gtlvayexnl.html

[Q65] 回滚事务
来源：http://hz.fengsongda.top/gtygyyjosg.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtjjllrbme.html

[Q66] 行锁查询
来源：http://hz.ivvv.top/gtkasrbcvj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtzwsiljpd.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtfietbpcp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yonumen.top/gtgtydwkvz.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gtdrwcllji.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtmdpzhyic.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtafzvpdei.html

[Q69] 查看执行计划
来源：http://hz.sxryk.cn/gtoqifmmmo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tian-w.cn/gtavvnoyrs.html

[Q70] 更新统计信息
来源：http://hz.smart0.xyz/gtwccqqkks.html

ANALYZE TABLE users;
来源：http://hz.ywan-chungtsiang.top/gtrqroipks.html

[Q71] 查看建表语句
来源：http://hz.yangfankeji.com/gttboumkyq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jqgfzy.top/gtnmiconub.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtbszfhasd.html

SHOW INDEX FROM users;
来源：http://hz.shangyingyoupin.top/gtbrphramp.html

[Q73] 查看表状态
来源：http://hz.yongpay.top/gtgpmlgpga.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangkeji.top/gtxzecshfh.html

[Q74] 强制使用索引
来源：http://hz.yuanzhike.top/gtooxerxjc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.quarkkingdee.top/gtliylkxbl.html

[Q75] 日期格式化
来源：http://hz.wangdashe.top/gtrtbsxpqe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtkkinfipt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dianchejie.cn/gtzldjpamw.html

[Q76] 按天统计
来源：http://hz.316326.xyz/gtxwglyuwe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yongpay.top/gtgyjelpgw.html

[Q77] 时间加减
来源：http://hz.daxiang520.top/gtwgmztoam.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gthkznlewe.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtzcunhpry.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtajqqailk.html

[Q79] 字符串拼接
来源：http://hz.yonumen.top/gtjiexnmoe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258888.top/gtvuudoblf.html

[Q80] 字符串截取
来源：http://hz.yj202588.top/gtatxwcliw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.kuanghao11.cn/gtcfvhcmer.html

[Q81] 字符串替换
来源：http://hz.vqdsnc.cn/gtzsrlvrrk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtvsjhyphe.html

[Q82] 字符长度与字节长度
来源：http://hz.gotoacloud.top/gtkfsfwbix.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtdtlgvhgj.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gtwsqhqwnw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gtjxwnnzov.html

[Q84] 去除首尾空格
来源：http://hz.ivvv.top/gtsnmvpwsz.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtrsozqiso.html

[Q85] 数值取整
来源：http://hz.birdmap.top/gtemdevhpk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhijiandao.cn/gtvdcrpdsm.html

[Q86] 读取 JSON 字段
来源：http://hz.xinyue.icu/gtiqvxzour.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtmuliunnc.html

[Q87] JSON 字段做条件
来源：http://hz.cdnleiting.top/gtltniuwep.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydjk.org.cn/gtvlasjwmf.html

[Q88] 行转列（条件聚合）
来源：http://hz.sufxvd.cn/gtgwgfcijw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.haohaochexian.top/gtuvoytgcu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cdnleiting.top/gtdkfeefrx.html

[Q89] 判断表是否存在
来源：http://hz.hammf.cn/gtuhuafdks.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gttyvyvapb.html

[Q90] 生成序号列
来源：http://hz.zhongyouzk.top/gtkipqpted.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gthnghkjhf.html

================================================================================
来源：http://hz.aibaodan.cn/gtzyfuzgsj.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtrimdliwi.html

================================================================================
来源：http://hz.316326.xyz/gtdlmmotgk.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtxgnhpdbj.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtlavqxapc.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtlyiwuwvz.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gtmzsasbos.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtcovllgxv.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtgzfxjkuz.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gtahzfndwo.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtkqxigahk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tianlin.xyz/gtyffxbntk.html

[R05] 参数默认值
来源：http://hz.shangyingyoupin.top/gtdodyiklt.html

name="${1:-default}"
来源：http://hz.ydzc1.top/gtuoddglfy.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtzaxrtqlg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtbthimbge.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtdoikbxcg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dianchejie.cn/gtgjfeuxoz.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtmzbghniy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shuidangran.top/gtyvtpkodo.html

[R09] 字符串比较
来源：http://hz.dashuyun.cn/gtjhwbccgh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cdnleiting.top/gtbwpgonnr.html

[R10] 正则匹配
来源：http://hz.jinqigfzy.top/gtqoxyzzvk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.feifeiyinyue.top/gtyhiteohy.html

[R11] case 多分支
来源：http://hz.ivvv.top/gtwpwbnxya.html

case "$1" in
来源：http://hz.jinqigufen.top/gtgcqnicqj.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtymarzeep.html

stop)  echo "停止" ;;
来源：http://hz.cdnleiting.top/gtnlrypcjo.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gtroxbikvz.html

esac
来源：http://hz.redwolf501.top/gtrmaawduh.html

[R12] for 遍历文件
来源：http://hz.shzxlz.cn/gtbrmmdiqe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hongshengwenyu.top/gttysgetaf.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gtfnwotudr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtwiofwcjx.html

[R14] C 风格 for
来源：http://hz.hnqzz.top/gteymbvbcr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ehwqpu.com/gtaerdykcl.html

[R15] while 逐行读文件
来源：http://hz.gogol.net.cn/gtxfubjxml.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gttqfkqwkz.html

[R16] until 等待条件
来源：http://hz.kuanghao11.cn/gtcogpxxgm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtdhltldlo.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtlvtejxvs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gtpiigodzb.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gtdoccgigi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenzaomai.com/gtiuxhhcwr.html

[R19] 数组长度
来源：http://hz.shanyushiyangtech.top/gtaonlzmkq.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtokeztyxh.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtqnyunkyl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtvodumjxi.html

[R21] 字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtiratoupv.html

echo "${#s}"
来源：http://hz.pengpengdd.cyou/gtmtnudian.html

[R22] 截取子串
来源：http://hz.pengpengdd.cyou/gtetkucasa.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtksqecdmg.html

[R23] 字符串替换
来源：http://hz.yueranfly.top/gtevdpldkf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtxjeedpnp.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtvotbsrdf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtkrwphpuk.html

[R25] 去后缀 / 去前缀
来源：http://hz.yvedp.cn/gtpajactgg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gtqczdhfyo.html

[R26] 命令替换
来源：http://hz.havefunace.top/gtdmqpiyyu.html

now=$(date +%F); echo "$now"
来源：http://hz.meibo888.top/gtislcuihk.html

[R27] 算术展开
来源：http://hz.yuxming.cn/gtzhuerddu.html

echo $((1 + 2 * 3))
来源：http://hz.nanxinkj.top/gtsppnxzvj.html

[R28] 浮点运算
来源：http://hz.andypj.xyz/gtszwtjxko.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtsoabquvb.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtdpfkwnqw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtatahqlrj.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtchladmko.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtjfbrgxly.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gtojlrylxj.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydjk.org.cn/gtpapqqlnn.html

[R32] 参数个数校验
来源：http://hz.tanke756.top/gthhvuocwz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnxiangtu.top/gtvumndlsm.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtfpjdzupd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtehtcejkh.html

[R34] 退出时清理
来源：http://hz.hywenlv.cn/gtloeeutse.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtgfmxggwy.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtjswbyltu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtskgtochc.html

[R36] 并发执行多个任务
来源：http://hz.gzhubu.top/gthyaouzww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtwbqmfabg.html

[R37] 把输出赋给变量
来源：http://hz.zhiwuduotai.top/gtjcqofduq.html

files=$(ls -1)
来源：http://hz.ydzc1.top/gtwzbhqjck.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtxdnzlptt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.kuanghao11.cn/gtjknptikl.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtxtchgque.html

cmd > out.log 2>&1
来源：http://hz.yuxming.cn/gtmcaoapom.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gtqybemrtw.html

echo "log" >> out.log
来源：http://hz.jqgufenzy.top/gtxgrrfapr.html

[R41] 丢弃输出
来源：http://hz.jinqigufen.top/gtfmlbmkgj.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gttdjvoswg.html

[R42] 输入重定向
来源：http://hz.dianchejie.cn/gtzhoalomd.html

wc -l < a.txt
来源：http://hz.daxiang520.top/gtyfdgnpdk.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtoaxcgxck.html

find . -name "*.log" -type f
来源：http://hz.hnxiangtu.top/gtmbxebmrt.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtcmkeysdz.html

find . -mtime -7 -type f
来源：http://hz.meibo888.top/gtkpznluzk.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtvglncvbk.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gtcwgqswwx.html

[R46] 递归替换文件内容
来源：http://hz.jqgfzy.top/gthqfvcdis.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daria6918.cn/gttrpamkkr.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gtfwolxais.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gtgaermszq.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtfxtoaobi.html

awk '{print $1, $3}' a.txt
来源：http://hz.yongpay.top/gtwtpuydad.html

[R49] awk 带条件
来源：http://hz.yanxiufei.cn/gtnmijwbfm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtbgapmzzb.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gtlqfzqvqp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuanzhike.top/gtfqhuoulv.html

[R51] 排序去重取前几
来源：http://hz.nanxuanxn.top/gtslqpmppt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xinyue.icu/gtghcdzvvi.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtmucdcxhx.html

wc -l a.txt
来源：http://hz.xuetiantiany.cn/gtikulcswq.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtdanaahax.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinghuilouyu.cn/gtqqdvzohc.html

[R54] 比较两个文件
来源：http://hz.zhiwuduotai.top/gteghlxsyo.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtcjmdpfek.html

[R55] 压缩与解压
来源：http://hz.yanxiufei.cn/gtkkgrbjtx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gtmkxkreoa.html

[R56] 远程拷贝
来源：http://hz.aizwys.cn/gtmxvowkit.html

scp file user@host:/path/
来源：http://hz.yj202588.top/gtckiefxsf.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtbzsplujw.html

ssh user@host 'uptime'
来源：http://hz.jinghuilouyu.cn/gtguldrnwr.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtkphcucci.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ivvv.top/gtarupxgsv.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtiivgnpxm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuanzhike.top/gtmasbajwo.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtajrxksav.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shzxlz.cn/gtabmultlb.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gtortdwdqa.html

df -h;  du -sh *
来源：http://hz.pycfn.com/gtyfuuolvr.html

[R62] 找最占空间的文件
来源：http://hz.tanke756.top/gtheqwqgyv.html

du -ah . | sort -rh | head -10
来源：http://hz.xuanzx.com/gtrdouxdxm.html

[R63] 内存与进程
来源：http://hz.meibo888.top/gtpcnicrlb.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gtgtbqqvuh.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtnlerycne.html

kill -9 $(pgrep -f app.py)
来源：http://hz.316326.xyz/gtppkngztz.html

[R65] 查看端口占用
来源：http://hz.yvedp.cn/gtffnmblry.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gttzotbwwe.html

[R66] 定时任务
来源：http://hz.sysykeji.top/gtcukcdxhz.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtcgjekmre.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtledafkgd.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtqpvrfipc.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtnvljcnjf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinqigfzy.top/gtgvvhagsx.html

[R69] 生成随机密码
来源：http://hz.feifeiyinyue.top/gtdlezsddf.html

head -c 16 /dev/urandom | base64
来源：http://hz.iojbl.cn/gtivdmuafq.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtwfkgsutx.html

date +%s;  date -d @1700000000
来源：http://hz.hongshengwenyu.top/gtpwnosqsi.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtjgyrjjfx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hysaishi.cn/gteqvvjcda.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtuorxzywq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yvedp.cn/gtefujffjp.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtympkdgkj.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtxacdapfl.html

[R74] 批量重命名
来源：http://hz.chenlongwang.top/gtvocfrxlj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yanxiufei.cn/gtemyqacqu.html

[R75] 导出环境变量
来源：http://hz.yonumen.top/gtkwmcrwio.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigufen.top/gtjbbufioz.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gtzoztjtou.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtwxuijsnm.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtdkezlcus.html

read -rp "请输入: " ans
来源：http://hz.zhixingplan.top/gtyjjdifax.html

[R78] 交互式菜单
来源：http://hz.0kj1m.cn/gthnxxnmxz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtnpktfuzy.html

[R79] 解析命令行选项
来源：http://hz.shangyingyoupin.top/gtsbamxoqx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtrhnbgdrv.html

[R80] 查看脚本执行耗时
来源：http://hz.zycfv.cn/gtlfxhwmvi.html

time ./run.sh
来源：http://hz.yuanzhike.top/gtbqggmyhk.html

================================================================================
来源：http://hz.zhengqikj.top/gtzhlpevix.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtshrqxgiy.html

================================================================================
来源：http://hz.zhengqikj.top/gtnfnfdqof.html

[S01] C：Hello World
来源：http://hz.jyoumei.cn/gtxnevtjtc.html

#include <stdio.h>
来源：http://hz.cheryme.top/gthdmkazqj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtanvtwvyf.html

[S02] C：变量与格式化输出
来源：http://hz.9152youxi.cn/gtkutoajmi.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtvuapcydv.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gtisiobigd.html

int x; scanf("%d", &x);
来源：http://hz.yanxiufei.cn/gtidduhxrc.html

[S04] C：字符串复制
来源：http://hz.bjfxy.top/gtltnhyvno.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hammf.cn/gthcgrhzvu.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gtqplbpnwf.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtjfiihflj.html

[S06] C：字符串比较
来源：http://hz.shuidangran.top/gtrclpozxd.html

strcmp(a, b) == 0
来源：http://hz.zycfv.cn/gtqubkujuq.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gthwmpdjvn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ivvv.top/gtdjchtstz.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtontiucwv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtqaqdeevi.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtahhpwing.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gogol.net.cn/gtqnzrasqh.html

[S10] C：指针与解引用
来源：http://hz.haohaochexian.top/gtuufjutkb.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtnvlsrpuh.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtrqeuwskq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gotoacloud.top/gtswsurczb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.redwolf501.top/gtpzajsdij.html

fclose(f);
来源：http://hz.hnqzz.top/gtoskercdx.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtmlbzjukq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangdashe.top/gtwtagtdmr.html

[S13] C：宏定义
来源：http://hz.jlsjyb.cn/gtmbesaocm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtdafthxrf.html

[S14] C：枚举
来源：http://hz.tian-w.cn/gtpplvkkai.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenzaomai.com/gtqtmldrbj.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gthtwgyuqo.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtogfrwcih.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtynicjdhs.html

x |= (1 << 3);
来源：http://hz.daria6918.cn/gtboodkray.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtbxtwtssi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yanxiufei.cn/gtwlktckhr.html

[S18] C：命令行参数
来源：http://hz.quarkkingdee.top/gttwanuown.html

int main(int argc, char **argv)
来源：http://hz.gogol.net.cn/gttndzzjko.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtsbbrhhbc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtlhipqnzj.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtzgapntzn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtjutcgdnk.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gtjpvffcpt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtcpphwiuq.html

[S22] C：字符串转数字
来源：http://hz.yj20258888.top/gtpzbinpav.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtdxpmcsxg.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gtoblbulgf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ppjwa.cn/gtlunqtehz.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtjofuvfzs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gtzpwrroof.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gtdovzytfx.html

memcpy(dst, src, n);
来源：http://hz.andypj.xyz/gtihfyiais.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtdlpeobri.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtfwovjtuo.html

[S27] C：定义常量
来源：http://hz.redwolf501.top/gtpkjmsrvn.html

const double PI = 3.14159;
来源：http://hz.haohaochexian.top/gtomandhvq.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtozxevyir.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtacyxdhdn.html

[S29] C：变参函数
来源：http://hz.ivvv.top/gtzvkcdgqo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtdgxhxtke.html

[S30] C：头文件保护
来源：http://hz.jinqigfzy.top/gtukcykvjf.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtealqbsds.html

#define X_H
来源：http://hz.sweek.top/gttewxfvtl.html

#endif
来源：http://hz.ppjwa.cn/gtsdgtsexw.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtxlciqreh.html

#include <iostream>
来源：http://hz.sysykeji.top/gtqbjztxmb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtemibpxgl.html

[S32] C++：字符串
来源：http://hz.zhijiandao.cn/gtaojrdxlo.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxuanxn.top/gtuzjqynsp.html


<!-- 参考信息 -->