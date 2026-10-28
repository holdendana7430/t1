代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtroauluum.html

[Q60] 取上一行 / 下一行
来源：http://hz.sweek.top/gtefvjsolm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtcjknmong.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.haohaochexian.top/gtrxeyyyoh.html

[Q61] 移动平均
来源：http://hz.andypj.xyz/gtjsjycewc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtytcoovbs.html

[Q62] 分组占比
来源：http://hz.cdnleiting.top/gtkbdcaotj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtxwvkfyqh.html

[Q63] 开启事务
来源：http://hz.ehwqpu.com/gtdavheznb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtmzfdkkmm.html

[Q64] 提交事务
来源：http://hz.jqgfzy.top/gtjltxcrmo.html

COMMIT;
来源：http://hz.shanyushiyangkeji.top/gtffixgzkm.html

[Q65] 回滚事务
来源：http://hz.gzhubu.top/gtyffkwdjb.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtiayckdmq.html

[Q66] 行锁查询
来源：http://hz.xylfe.cn/gtabuikenh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhengqikj.top/gttkhgqlim.html

[Q67] 设置隔离级别
来源：http://hz.dashuyun.cn/gtfudnauoc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gtcxdlxwjg.html

[Q68] 保存点
来源：http://hz.yueranfly.top/gtgffyixmn.html

SAVEPOINT sp1;
来源：http://hz.mhx1999.top/gtshrbrrkr.html

ROLLBACK TO sp1;
来源：http://hz.snrcjt.cn/gtzmysdbrz.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtvihmmjwv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.haohaochexian.top/gtdxlurinw.html

[Q70] 更新统计信息
来源：http://hz.dashuyun.cn/gtabrrxjvo.html

ANALYZE TABLE users;
来源：http://hz.guannengcc.top/gtwxitryba.html

[Q71] 查看建表语句
来源：http://hz.mhx1999.top/gtgyoowywe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258.top/gtcutwogup.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtnxbvvmya.html

SHOW INDEX FROM users;
来源：http://hz.sufxvd.cn/gtmllyggct.html

[Q73] 查看表状态
来源：http://hz.fzhhl.top/gtqevpfrya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gaohongyu789.top/gtkbyudzcw.html

[Q74] 强制使用索引
来源：http://hz.jqgfzy.top/gtyyfhcmpl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ywan-chungtsiang.top/gtyjpsemdz.html

[Q75] 日期格式化
来源：http://hz.guannengcc.top/gtrihxysgv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.snrcjt.cn/gtqjsrywyh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cqqwz.cn/gtewnhuivl.html

[Q76] 按天统计
来源：http://hz.chenzaomai.com/gtbdebyqnc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtqvehuryc.html

[Q77] 时间加减
来源：http://hz.gogol.net.cn/gtkhxalmqz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtoqzhpakz.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtrplapwtm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gtxqyerxpe.html

[Q79] 字符串拼接
来源：http://hz.nwbrower.top/gtesprreua.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daria6918.cn/gtbnbpkpuh.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtryjwdabv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yvedp.cn/gtdlnbkahi.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtzasxxrsq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fengsongda.top/gtogjugyvm.html

[Q82] 字符长度与字节长度
来源：http://hz.yangfankeji.com/gtyejopawb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtqooujaso.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtlnpnmkat.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtemizunwr.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtotyutstf.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtweayolxo.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtummdkeyp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtdodsmtbw.html

[Q86] 读取 JSON 字段
来源：http://hz.ydjk.org.cn/gtcqumdbnq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ywan-chungtsiang.top/gttczotpay.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtjaiersoe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gtosjsatnx.html

[Q88] 行转列（条件聚合）
来源：http://hz.daria6918.cn/gtmsujgild.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangtech.top/gtbkabjmtn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtosvvhjyg.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtpjafvsyh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtszdokpdc.html

[Q90] 生成序号列
来源：http://hz.ppjwa.cn/gtelvbiymy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258888.top/gthximnqez.html

================================================================================
来源：http://hz.ehwqpu.com/gtldcsznqk.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtonlicqrm.html

================================================================================
来源：http://hz.dianchejie.cn/gthryfacdg.html

[R01] shebang 与严格模式
来源：http://hz.jinqigfzy.top/gtktaqspec.html

#!/usr/bin/env bash
来源：http://hz.jyoumei.cn/gtdarlychd.html

set -euo pipefail
来源：http://hz.jlsjyb.cn/gtcdsipyjh.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gtxooqnlqh.html

name="Tom"; echo "$name"
来源：http://hz.snrcjt.cn/gtzjfnormb.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtyytqglyn.html

readonly PI=3.14
来源：http://hz.tian-w.cn/gtpfwujrsn.html

[R04] 位置参数
来源：http://hz.sweek.top/gtmjjhztnc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenzaomai.com/gtrhppjmgz.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtdfztbdnj.html

name="${1:-default}"
来源：http://hz.yvedp.cn/gtfiybpljg.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtyrfrfoej.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtrebdytta.html

[R07] if 判断文件
来源：http://hz.sweek.top/gtvhgmrhvb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tanke756.top/gtjhlfuccz.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gtuckrxfru.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtbwufpelk.html

[R09] 字符串比较
来源：http://hz.daria6918.cn/gtkycqjjbe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gtkqapsvjj.html

[R10] 正则匹配
来源：http://hz.jlsjyb.cn/gtofusyvet.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.bjfxy.top/gtbmwqdtmu.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtfhkbkmrb.html

case "$1" in
来源：http://hz.zdqjudy.top/gtxzypeqcj.html

start) echo "启动" ;;
来源：http://hz.guannengcc.top/gtrpqjsyeu.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gtmhojxljd.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gtnrjffczl.html

esac
来源：http://hz.xingfuxueyuan.xyz/gtaqllabtz.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gthvuurepi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtvoflcylw.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtpxzmjcef.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtpjzimxxg.html

[R14] C 风格 for
来源：http://hz.svipenyu.cn/gtdcjfymgm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtlxvjgggx.html

[R15] while 逐行读文件
来源：http://hz.yuxming.cn/gtogcpmpav.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtdyatpbnn.html

[R16] until 等待条件
来源：http://hz.svipenyu.cn/gtlyyvqmlg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtoarynqkm.html

[R17] 数组定义与取值
来源：http://hz.cucudq.cn/gtkbiwlogf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtjypzofwn.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gthtdgixtp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zdqjudy.top/gtggqenolf.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtqlpmbvtr.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtolquwzon.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtrupwiwhs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtaixetghd.html

[R21] 字符串长度
来源：http://hz.316326.xyz/gtmjifauri.html

echo "${#s}"
来源：http://hz.meibo888.top/gtokphlnub.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtegsbrvhj.html

echo "${s:0:5}"
来源：http://hz.pengpengdd.cyou/gtvcmlpsix.html

[R23] 字符串替换
来源：http://hz.redwolf501.top/gthcahpmpc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.mhx1999.top/gtkadvqcho.html

[R24] 大小写转换
来源：http://hz.havefunace.top/gtkljsgsfx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ppjwa.cn/gtsywdjbdf.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtneaiezfk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nwbrower.top/gtjhrtyqiz.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtygpkfoti.html

now=$(date +%F); echo "$now"
来源：http://hz.xuanzx.com/gtebqonnas.html

[R27] 算术展开
来源：http://hz.shangyingyoupin.top/gtaokgaqeq.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtdqeavzhv.html

[R28] 浮点运算
来源：http://hz.smart0.xyz/gtlfoldlgo.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtohtojdhu.html

[R29] 定义函数
来源：http://hz.smart0.xyz/gtesrxynmd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtwmyyjlun.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtetxpacsu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenjidiqi.icu/gtruiavoon.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gtnpgmfbea.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtcesyfgvm.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtlwxmpqdc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cashguo.top/gtuybjfgqc.html

[R33] 捕获错误并提示行号
来源：http://hz.tianlin.xyz/gtlnjwqafh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gtoiqkgrqn.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtfipemjhx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtwoyuqzlc.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gtozfbfhdl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtnfjbialg.html

[R36] 并发执行多个任务
来源：http://hz.jinqigfzy.top/gthepfliqm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gtowwwyqkp.html

[R37] 把输出赋给变量
来源：http://hz.shzxlz.cn/gtewbbhaml.html

files=$(ls -1)
来源：http://hz.yj202588.top/gticrgaktt.html

[R38] 管道串联
来源：http://hz.52xcode.cn/gtuqnumyid.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtotjspgfd.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtazudqcjr.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtgifmxupm.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtuavfaifb.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtwyhrbfta.html

[R41] 丢弃输出
来源：http://hz.hnxiangtu.top/gtkqdwpizm.html

cmd >/dev/null 2>&1
来源：http://hz.yangfankeji.com/gtmetezjlg.html

[R42] 输入重定向
来源：http://hz.316326.xyz/gtghjgqspa.html

wc -l < a.txt
来源：http://hz.jinyuanbaomall.cn/gtsvwkctrf.html

[R43] 按名字查找文件
来源：http://hz.0kj1m.cn/gtpjwojhsj.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtajohcmoq.html

[R44] 按修改时间查找
来源：http://hz.52xcode.cn/gtccegkgat.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gtofggmxrf.html

[R45] 批量删除
来源：http://hz.gotoacloud.top/gtpnbfkrsl.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gtzkgftnay.html

[R46] 递归替换文件内容
来源：http://hz.ppjwa.cn/gtfmiqwyfr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gthfrytxgv.html

[R47] sed 单行替换
来源：http://hz.jqgfzy.top/gtidsbjckw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtukabxuei.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtbwanzjjb.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenjidiqi.icu/gtolipdrmg.html

[R49] awk 带条件
来源：http://hz.xinyue.icu/gtvfivyeml.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gttidsgqjt.html

[R50] awk 求和
来源：http://hz.yvedp.cn/gtixqnxnmc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangdashe.top/gtthsdvmkd.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtvhymjeeu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgfzy.top/gtygoyxiuv.html

[R52] 统计行数
来源：http://hz.cdnleiting.top/gtbqzktumh.html

wc -l a.txt
来源：http://hz.daxiang520.top/gtstlyrdaa.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtgvetaqyl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangkeji.top/gtizrgznla.html

[R54] 比较两个文件
来源：http://hz.316326.xyz/gtkuynouhv.html

diff a.txt b.txt
来源：http://hz.jqgufenzy.top/gttqkuxwnm.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtbcxyugvv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jyoumei.cn/gtkecsbopj.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gthrfcymrl.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gtywrpjlrw.html

[R57] 远程执行命令
来源：http://hz.zhengqikj.top/gtvkbzgeex.html

ssh user@host 'uptime'
来源：http://hz.jinqigufen.top/gtlighouau.html

[R58] 下载文件
来源：http://hz.cucudq.cn/gtxcmkjtco.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nwbrower.top/gtspuxvrys.html

[R59] 发 POST JSON
来源：http://hz.fzhhl.top/gtnyukheue.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtmrwlephq.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtcoclgkki.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuanzx.com/gtfisknqoo.html

[R61] 磁盘占用
来源：http://hz.tian-w.cn/gtxmueidep.html

df -h;  du -sh *
来源：http://hz.fzhhl.top/gtkdhdhhcg.html

[R62] 找最占空间的文件
来源：http://hz.hnqzz.top/gtiwfsmwhj.html

du -ah . | sort -rh | head -10
来源：http://hz.smart0.xyz/gtrplgzchj.html

[R63] 内存与进程
来源：http://hz.pycfn.com/gtfzdmwrmp.html

free -h;  ps aux | grep nginx
来源：http://hz.dashuyun.cn/gtkcswvyef.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtgzbgqres.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtklveeaxj.html

[R65] 查看端口占用
来源：http://hz.ybcxt.top/gtqiyydgia.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.bjfxy.top/gtxorayfqe.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtmihtmdbs.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gtwvxrwqsu.html

[R67] 生成随机十六进制串
来源：http://hz.cdnleiting.top/gtduhaurxr.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtfyyxqjhv.html

[R68] 计算文件校验值
来源：http://hz.wangshuangyany.cn/gtipogtysk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gtksvfgnhl.html

[R69] 生成随机密码
来源：http://hz.ybcxt.top/gtzgzatjbt.html

head -c 16 /dev/urandom | base64
来源：http://hz.birdmap.top/gtlluyfyzj.html

[R70] 时间戳与互转
来源：http://hz.yvedp.cn/gtvrmhxchv.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gtodjtrghk.html

[R71] 日期格式化
来源：http://hz.zhoulong.xyz/gtcvgisfgf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtnxokenxk.html

[R72] 等待端口就绪
来源：http://hz.zdqjudy.top/gtmzwityne.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cheryme.top/gtkygrydqr.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gtqrwabxud.html

split -l 1000 big.log part_
来源：http://hz.jqgufenzy.top/gtqsbqjjiv.html

[R74] 批量重命名
来源：http://hz.mhx1999.top/gtqvkeplon.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtwoamqmgb.html

[R75] 导出环境变量
来源：http://hz.hywenlv.cn/gtrrebqjil.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yongpay.top/gtignrjayo.html

[R76] 使用临时文件
来源：http://hz.zhixingplan.top/gtwcspjpbv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gteihlrkmt.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gtfsqenbbc.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gtmlwmevch.html

[R78] 交互式菜单
来源：http://hz.cucudq.cn/gtyyibakxx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtoiglfogk.html

[R79] 解析命令行选项
来源：http://hz.cdnleiting.top/gtnvfepcxg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtypzkxiwn.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gtahlepgii.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtefjjxvbx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtipzgiylk.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtphkytxas.html

================================================================================
来源：http://hz.zhoulong.xyz/gtthhpxsdy.html

[S01] C：Hello World
来源：http://hz.daria6918.cn/gtnplvoghd.html

#include <stdio.h>
来源：http://hz.aibaodan.cn/gtpvrcxyha.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gotoacloud.top/gtolepqhrr.html

[S02] C：变量与格式化输出
来源：http://hz.hammf.cn/gtlckfuvip.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtsyrkkrwk.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gtsvmvioee.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtdiultvbm.html

[S04] C：字符串复制
来源：http://hz.daria6918.cn/gtxwmankeh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtkmxcrxji.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gthxtcdqnq.html

strlen(s)
来源：http://hz.zhijiandao.cn/gtbhczxixm.html

[S06] C：字符串比较
来源：http://hz.jqgfzy.top/gtxdflktkk.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangtech.top/gtdasvpdhz.html

[S07] C：数组遍历求和
来源：http://hz.svipenyu.cn/gtbjpijhfa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ehwqpu.com/gtfwpuzlnx.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtfxtcwzin.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.iojbl.cn/gtkqaetmks.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gtbbfrwldf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gtruezulux.html

[S10] C：指针与解引用
来源：http://hz.yuanzhike.top/gtfgtpexul.html

int *p = &a;  *p = 5;
来源：http://hz.mhx1999.top/gtvvfluulk.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtpeaugdgn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.mhx1999.top/gtcpvdipkq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnxiangtu.top/gtealtjlqs.html

fclose(f);
来源：http://hz.sxryk.cn/gtnurrckga.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gttqkfopos.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtvrcvggjx.html

[S13] C：宏定义
来源：http://hz.jinqigufen.top/gtljeftrjd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gtpmearahw.html

[S14] C：枚举
来源：http://hz.zycfv.cn/gtgelmuviu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yonumen.top/gtrpigdawg.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtgicxdbol.html

(double) a / b
来源：http://hz.jinqigufen.top/gtqewdsrif.html

[S16] C：位操作置位
来源：http://hz.kuanghao11.cn/gtcyspagco.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtsfvrrsct.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gtwoaodgrk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gtscijfdkr.html

[S18] C：命令行参数
来源：http://hz.cheryme.top/gtezblgpgn.html

int main(int argc, char **argv)
来源：http://hz.chenzaomai.com/gtaajuykhb.html

[S19] C：快速排序
来源：http://hz.ppjwa.cn/gtzjazrvtm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtugwvzswy.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gtyuktjgjs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtevuvrzsy.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gthunwatrh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jiagoushi.top/gtewlbpuhx.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtxpimcmrl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtzbxvnton.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtxjqajmfp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gzhubu.top/gtrewgrxmc.html

[S24] C：获取本地时间
来源：http://hz.fzhhl.top/gtmghtbxlk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhaomingkeji.xyz/gtcfsqxszw.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtmtebpjjg.html

memcpy(dst, src, n);
来源：http://hz.zdqjudy.top/gtjpndakus.html

[S26] C：内存清零
来源：http://hz.nanxuanxn.top/gteresctsx.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtasxjdwzd.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gtifyefoiz.html

const double PI = 3.14159;
来源：http://hz.0kj1m.cn/gtbinlmmyu.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gtlzxfrtmg.html

static int counter = 0;
来源：http://hz.yj20258888.top/gtmrsexrfi.html

[S29] C：变参函数
来源：http://hz.sufxvd.cn/gttltuizxd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.snrcjt.cn/gtwvmkvatn.html

[S30] C：头文件保护
来源：http://hz.shangyingyoupin.top/gtwfmrrkdr.html


<!-- 参考信息 -->