代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hysaishi.cn/gtpkcmmrng.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtksndhwxy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtgcksazni.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gtudcflbgg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtchtyndkw.html

[Q52] 删除指定行
来源：http://hz.jinghuilouyu.cn/gtajvnrgby.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zdqjudy.top/gthihplybw.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gthkozftup.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhongyouzk.top/gtdpmiuvkz.html

[Q54] 清空表
来源：http://hz.nwbrower.top/gtveiicetp.html

TRUNCATE TABLE logs;
来源：http://hz.zhijiandao.cn/gtlchhkufd.html

[Q55] 排名（并列占位）
来源：http://hz.nwbrower.top/gtxjronazu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtjkpqybjb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shuidangran.top/gtakwoqsjc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtmlibmekx.html

[Q57] 行号
来源：http://hz.hongshengwenyu.top/gtkpcvbcaf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.snrcjt.cn/gtrnjxwlmm.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtpcgzbtor.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tian-w.cn/gtfsyqtivo.html

[Q59] 分组内累计
来源：http://hz.yonumen.top/gtyjvjoaoz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtmpajsebj.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtzoeluwjk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhixingplan.top/gthmefmaew.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtrbghmuee.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtqdacdkfg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtklvndlec.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gtipisbodt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtesjvdhwh.html

[Q63] 开启事务
来源：http://hz.chenzaomai.com/gtpvviztxn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dianchejie.cn/gtacgoqtcm.html

[Q64] 提交事务
来源：http://hz.bjfxy.top/gtwvvnehxz.html

COMMIT;
来源：http://hz.aibaodan.cn/gteowqhhmu.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtvxxssvlj.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gtwosmsrxn.html

[Q66] 行锁查询
来源：http://hz.zdqjudy.top/gtqfkmobet.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtnuplhrva.html

[Q67] 设置隔离级别
来源：http://hz.aizwys.cn/gtmfctisdf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sufxvd.cn/gtctbdllzh.html

[Q68] 保存点
来源：http://hz.aibaodan.cn/gtlkbloswc.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtfwepakxj.html

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtpwmiufme.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtnjygcmbj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cheryme.top/gteglzspww.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtbxtawbwk.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gtjllzkmbe.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtwmcsggdf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.316326.xyz/gtldbxxeae.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtdoeyzyte.html

SHOW INDEX FROM users;
来源：http://hz.c1oappe.top/gtjetttzok.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtitedmesl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtspzedcbt.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtmkifxatv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuxming.cn/gtjrpvwesd.html

[Q75] 日期格式化
来源：http://hz.zhongyouzk.top/gtbnwjxxec.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtdgauxqmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtygwwovdg.html

[Q76] 按天统计
来源：http://hz.yvedp.cn/gtlrafgapy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.svipenyu.cn/gthzzitcwj.html

[Q77] 时间加减
来源：http://hz.havefunace.top/gtpfdqtvzn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.9152youxi.cn/gtcqaqwfnu.html

[Q78] 当前时间
来源：http://hz.zhijiandao.cn/gtacusgnne.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtnlbfgkfl.html

[Q79] 字符串拼接
来源：http://hz.shangyingyoupin.top/gtvuskmynp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tianlin.xyz/gtgxhllnjq.html

[Q80] 字符串截取
来源：http://hz.nwbrower.top/gtbtqzxkct.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.316326.xyz/gtcreieiaq.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtkchkxdqb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtsadaqweg.html

[Q82] 字符长度与字节长度
来源：http://hz.guannengcc.top/gtilkqktik.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtablbjnqe.html

[Q83] 大小写转换
来源：http://hz.tian-w.cn/gtdybgssqa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtikjmwpsz.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtffbacemj.html

SELECT TRIM(name) FROM users;
来源：http://hz.hammf.cn/gtfhgsflqg.html

[Q85] 数值取整
来源：http://hz.andypj.xyz/gtgghptixk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtpfjoyins.html

[Q86] 读取 JSON 字段
来源：http://hz.yj202588.top/gtwkdwrswr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xinyue.icu/gtnsxsrilj.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gttshhevla.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtuyrsijdf.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangshuangyany.cn/gtkusixdqk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pycfn.com/gtfpcjnpdt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xziqi.cn/gtzmsjbvja.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtxxjlfhjz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenlongwang.top/gtgnktxqlr.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtveyfewrf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.havefunace.top/gtrrqfqxkw.html

================================================================================
来源：http://hz.redwolf501.top/gtczzvcjjf.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtnjqzdzwd.html

================================================================================
来源：http://hz.guannengcc.top/gtueusqnuq.html

[R01] shebang 与严格模式
来源：http://hz.wangshuangyany.cn/gtagqfxpcc.html

#!/usr/bin/env bash
来源：http://hz.yuxming.cn/gtwpfarjzn.html

set -euo pipefail
来源：http://hz.9152youxi.cn/gtrzzczqhn.html

[R02] 变量赋值与使用
来源：http://hz.redwolf501.top/gtsmnotawa.html

name="Tom"; echo "$name"
来源：http://hz.andypj.xyz/gticpnwmzc.html

[R03] 只读变量
来源：http://hz.shanyushiyangtech.top/gtwpdqguyo.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtxszjjltb.html

[R04] 位置参数
来源：http://hz.gogol.net.cn/gtyrijcclx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cucudq.cn/gtvkajfhmi.html

[R05] 参数默认值
来源：http://hz.havefunace.top/gtogtznxvj.html

name="${1:-default}"
来源：http://hz.jinghuilouyu.cn/gtnksdbzyd.html

[R06] 判断命令是否存在
来源：http://hz.vqdsnc.cn/gtqqhlrtmn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtwcpxzgix.html

[R07] if 判断文件
来源：http://hz.tanke756.top/gtqlimdion.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuetiantiany.cn/gtrmpuxpdm.html

[R08] 数值比较
来源：http://hz.xziqi.cn/gtsogxpkpi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gtlxcecotz.html

[R09] 字符串比较
来源：http://hz.cdnleiting.top/gtcrdjlmav.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.svipenyu.cn/gtsgsryixn.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtzhzzdevu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gtouidemuw.html

[R11] case 多分支
来源：http://hz.hongshengwenyu.top/gtmnerscfb.html

case "$1" in
来源：http://hz.zhongyouzk.top/gtfdiyojkd.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangtech.top/gtkppbklix.html

stop)  echo "停止" ;;
来源：http://hz.hywenlv.cn/gtmejjhnqy.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtqekauebs.html

esac
来源：http://hz.aizwys.cn/gtrykfwylh.html

[R12] for 遍历文件
来源：http://hz.sxryk.cn/gtldxxjhjw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.svipenyu.cn/gthqrwflqe.html

[R13] for 计数循环
来源：http://hz.yj20258.top/gtmbjhrnnp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.daria6918.cn/gtsqjtjwul.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gtumygxdnz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zycfv.cn/gtwriejxgf.html

[R15] while 逐行读文件
来源：http://hz.xuanzx.com/gttuuapkis.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtgnwgbqph.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtjqvcxksi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtttjxbrqj.html

[R17] 数组定义与取值
来源：http://hz.zycfv.cn/gtbkbzpmhe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.feifeiyinyue.top/gtpchfytlj.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtbpuhitqn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shuidangran.top/gtnaucghag.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtnaaqezci.html

echo "${#arr[@]}"
来源：http://hz.yongpay.top/gtmnixhtlu.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtyayogzkx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.snrcjt.cn/gtxryitruk.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtclpnmvwt.html

echo "${#s}"
来源：http://hz.xylfe.cn/gtqvjduxtk.html

[R22] 截取子串
来源：http://hz.sysykeji.top/gtohiuouji.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtnbpioovi.html

[R23] 字符串替换
来源：http://hz.svipenyu.cn/gtvrdglyef.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cdnleiting.top/gtgcimprhq.html

[R24] 大小写转换
来源：http://hz.yvedp.cn/gtvoouabqn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.snrcjt.cn/gtexracxye.html

[R25] 去后缀 / 去前缀
来源：http://hz.feifeiyinyue.top/gtzgtqvmvc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigufen.top/gtvsyqbvwt.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtvxdxfiqz.html

now=$(date +%F); echo "$now"
来源：http://hz.ydzc1.top/gtxpvqhvtr.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtsrxgyhfq.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gtibwxwrqx.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtlkyypirv.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydzc1.top/gtmwdohfic.html

[R29] 定义函数
来源：http://hz.sxryk.cn/gtkmygvsqp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ehwqpu.com/gtpglvaozs.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtnzzoylba.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.svipenyu.cn/gtmhaorllh.html

[R31] 局部变量
来源：http://hz.chenzaomai.com/gtoqruhdsx.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtdtigoqck.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtpgsnchwi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuanzhike.top/gtvphvwksk.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtmuekqhfv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtwfzsrnmt.html

[R34] 退出时清理
来源：http://hz.shanyushiyangkeji.top/gtngljbzxn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtmufquvxh.html

[R35] 后台执行并等待
来源：http://hz.vqdsnc.cn/gtrlahhixm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydzc1.top/gtphsdibsr.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtjqyactsc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gogol.net.cn/gtoyhwxeqz.html

[R37] 把输出赋给变量
来源：http://hz.bjfxy.top/gtbjzwmaxj.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtchbvctma.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtdctoxrja.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sufxvd.cn/gtcsvccepe.html

[R39] 重定向标准输出与错误
来源：http://hz.ppjwa.cn/gtsjkiwpwh.html

cmd > out.log 2>&1
来源：http://hz.ivvv.top/gtbmxpyvzb.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtyatjlxpb.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtmpmhtvjd.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangkeji.top/gtipydscgr.html

cmd >/dev/null 2>&1
来源：http://hz.jlsjyb.cn/gtypzcywee.html

[R42] 输入重定向
来源：http://hz.mhx1999.top/gtnhkpnzun.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gttomuneno.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtpcsdcqol.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtkwghlhby.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gtfajrdymr.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtamowectf.html

[R45] 批量删除
来源：http://hz.sufxvd.cn/gtwfwocmbs.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtomwjysuj.html

[R46] 递归替换文件内容
来源：http://hz.quarkkingdee.top/gtplzftcgo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtzmccceyp.html

[R47] sed 单行替换
来源：http://hz.jqgfzy.top/gtxesbwyob.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gogol.net.cn/gtbtlglvgz.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtrtkdoagx.html

awk '{print $1, $3}' a.txt
来源：http://hz.ivvv.top/gtotalgumh.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtvwlgujea.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenlongwang.top/gtrgcycdgz.html

[R50] awk 求和
来源：http://hz.nwbrower.top/gttbjzycvw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtvyannbbz.html

[R51] 排序去重取前几
来源：http://hz.zdqjudy.top/gtkoymvvki.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.havefunace.top/gtxseoazgc.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtgthrhgbm.html

wc -l a.txt
来源：http://hz.cashguo.top/gtkbutnwpx.html

[R53] 查看文件头与实时尾
来源：http://hz.yanxiufei.cn/gtpbzcqqzo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hysaishi.cn/gtupuokslt.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtsspmynsi.html

diff a.txt b.txt
来源：http://hz.hongshengwenyu.top/gtsrsuexlr.html

[R55] 压缩与解压
来源：http://hz.guowangkeji.top/gtrynyccqm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sxryk.cn/gtbnnrzeec.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtnzgbqjeg.html

scp file user@host:/path/
来源：http://hz.dashuyun.cn/gtkakqzuuy.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gtrxviscvz.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtvgyeocwx.html

[R58] 下载文件
来源：http://hz.zhongyouzk.top/gtiodcajes.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtarkojjos.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gtzqieroff.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtshvrdfsq.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtpzilqdex.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yueranfly.top/gtodjqbsbq.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gtqljopqrk.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtnabtacgl.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtjiwmdwdz.html

du -ah . | sort -rh | head -10
来源：http://hz.zhengqikj.top/gtmrdydthu.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtltxfgmnv.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtelpgzggk.html

[R64] 结束进程
来源：http://hz.aizwys.cn/gtlpwihnbm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgufenzy.top/gtkspsbbth.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtxdcblpvj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gttrkkukwo.html

[R66] 定时任务
来源：http://hz.daria6918.cn/gtqmzclhtl.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gtpcqaoksq.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gteegvviha.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gticmgkzwi.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gtrqpcnmag.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuetiantiany.cn/gtgjpgucpf.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtlmpnwkxe.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtllyaynsz.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gtaxwkhtvd.html

date +%s;  date -d @1700000000
来源：http://hz.xziqi.cn/gtfffqgfkt.html

[R71] 日期格式化
来源：http://hz.ivvv.top/gttenkdwgn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangkeji.top/gttichipgw.html

[R72] 等待端口就绪
来源：http://hz.nanxinkj.top/gtyecfbqan.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jiagoushi.top/gtdgpjsuiy.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gtmgehmihx.html

split -l 1000 big.log part_
来源：http://hz.ppjwa.cn/gtbblbhhqr.html

[R74] 批量重命名
来源：http://hz.guannengcc.top/gtenfgwbnz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gtjwzxhvta.html

[R75] 导出环境变量
来源：http://hz.gaohongyu789.top/gtlxkyurfq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtjbfigbtd.html

[R76] 使用临时文件
来源：http://hz.kuanghao11.cn/gtlzszkabz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtfchygotq.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtiukihqph.html

read -rp "请输入: " ans
来源：http://hz.chenjidiqi.icu/gtzrgkaepe.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtpxtxgeuc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258.top/gtsvjkgtaf.html

[R79] 解析命令行选项
来源：http://hz.jinghuilouyu.cn/gtjtjosbau.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xingfuxueyuan.xyz/gtiudfoimj.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtarxnvsra.html

time ./run.sh
来源：http://hz.nwbrower.top/gthovtxxyd.html

================================================================================
来源：http://hz.ivvv.top/gtaydqgjzp.html

S. C / C++ 专题
来源：http://hz.xinyue.icu/gtxbntuzmy.html

================================================================================
来源：http://hz.xinyue.icu/gtpabfpktc.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtgchinyxp.html

#include <stdio.h>
来源：http://hz.yvedp.cn/gtswbqqvhv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtadpmopaf.html

[S02] C：变量与格式化输出
来源：http://hz.ivvv.top/gtmnxhcupc.html

int a = 10; printf("%d\n", a);
来源：http://hz.jlsjyb.cn/gtsvxrddsy.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gtqhegoayb.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtneryitzg.html

[S04] C：字符串复制
来源：http://hz.hongshengwenyu.top/gtbnbuiyfi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.feifeiyinyue.top/gtanhfermf.html

[S05] C：字符串长度
来源：http://hz.haohaochexian.top/gtuhqquxmv.html

strlen(s)
来源：http://hz.xingfuxueyuan.xyz/gtqyedpxyh.html

[S06] C：字符串比较
来源：http://hz.jyoumei.cn/gtjzpziffw.html

strcmp(a, b) == 0
来源：http://hz.fzhhl.top/gtjbhvrexx.html

[S07] C：数组遍历求和
来源：http://hz.316326.xyz/gtwyicgkli.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daxiang520.top/gtyncrtvsv.html

[S08] C：动态内存分配与释放
来源：http://hz.hfpthk.cn/gtxzspfork.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cdnleiting.top/gtzterkgsc.html

[S09] C：结构体定义与初始化
来源：http://hz.9152youxi.cn/gttgkswpfs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigufen.top/gtcpimbvez.html

[S10] C：指针与解引用
来源：http://hz.yj20258.top/gtggjdnllj.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtvczlkagr.html

[S11] C：逐行读文件
来源：http://hz.ybcxt.top/gtxcnqsvzj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtnxgqivkl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fengsongda.top/gtlljrdbhb.html

fclose(f);
来源：http://hz.yangfankeji.com/gtzkpkafui.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtvauklqrl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtaplirdvz.html

[S13] C：宏定义
来源：http://hz.zhijiandao.cn/gttoyajpdg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ehwqpu.com/gtbrlxpevq.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtlkjmwzib.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gtwmghszkv.html

[S15] C：类型转换
来源：http://hz.fzhhl.top/gtmmasjikx.html

(double) a / b
来源：http://hz.xziqi.cn/gtphcksvzm.html

[S16] C：位操作置位
来源：http://hz.ydjk.org.cn/gtfvfdbrfy.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtsiupedjf.html

[S17] C：安全拼接字符串
来源：http://hz.zdqjudy.top/gtkgnpxwgc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.quarkkingdee.top/gtxeuiedcc.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtgzxveblv.html

int main(int argc, char **argv)
来源：http://hz.hnqzz.top/gtbemomwlk.html

[S19] C：快速排序
来源：http://hz.jinghuilouyu.cn/gtywhlyeqn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtsumdsmmy.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtmiudnais.html


<!-- 参考信息 -->