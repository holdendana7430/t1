代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.zhaomingkeji.xyz/gtsgvjgbvx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtcoywbqki.html

[Q43] 标量子查询
来源：http://hz.316326.xyz/gtiqbxjmsu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtbhbulfad.html

[Q44] IN 子查询
来源：http://hz.birdmap.top/gtehzhyqkp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xylfe.cn/gtmaiholgm.html

[Q45] EXISTS 判断存在
来源：http://hz.zhiwuduotai.top/gtsulshxml.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtxgxwqisi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ehwqpu.com/gtyqqdwjsh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtckcwcmlv.html

[Q47] 与平均值比较
来源：http://hz.chenlongwang.top/gtfrvchkkr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gtqoqwmtna.html

[Q48] CTE 公用表表达式
来源：http://hz.wangdashe.top/gtxhjslfdq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.52xcode.cn/gtadmeorqs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtijtzgwuj.html

[Q49] 更新单行
来源：http://hz.cqqwz.cn/gtjrlzxkib.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtjtfuugef.html

[Q50] 批量更新
来源：http://hz.52xcode.cn/gtypqujzsj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtsxsylonr.html

[Q51] 用子查询更新
来源：http://hz.zhaomingkeji.xyz/gtaoplllem.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shzxlz.cn/gtsxggvbxb.html

[Q52] 删除指定行
来源：http://hz.shanyushiyangkeji.top/gtvrexyjej.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtegatsjyz.html

[Q53] 按条件删除
来源：http://hz.guowangkeji.top/gtgqcylyww.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtpmwdykac.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gttttpinza.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gtxpghhsye.html

[Q55] 排名（并列占位）
来源：http://hz.yangfankeji.com/gtxfcddare.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fzhhl.top/gtkiirqqye.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtraoosltm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shzxlz.cn/gtpypmomde.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtwzxpamla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gtqrkoqqjw.html

[Q58] 累计求和
来源：http://hz.jiagoushi.top/gtlhhmfrma.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenjidiqi.icu/gtwqjnhxiv.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtpjcvrjdr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gaohongyu789.top/gtpriutahi.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gtemqwjfxk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhiwuduotai.top/gtiwqzrvxw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtmdxighbz.html

[Q61] 移动平均
来源：http://hz.yuxming.cn/gtilbrlfdt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtmfbteeim.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gtudzkqbzu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtiybaziqb.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gthrgtebep.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhixingplan.top/gtnxtxaqmz.html

[Q64] 提交事务
来源：http://hz.tanke756.top/gtyxzxyrqy.html

COMMIT;
来源：http://hz.guannengcc.top/gtfqsdnpxo.html

[Q65] 回滚事务
来源：http://hz.0kj1m.cn/gtadgopdqm.html

ROLLBACK;
来源：http://hz.jqgfzy.top/gtvvscxvgb.html

[Q66] 行锁查询
来源：http://hz.hnxiangtu.top/gtpkjwozbj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xingfuxueyuan.xyz/gtxwmukkck.html

[Q67] 设置隔离级别
来源：http://hz.zdqjudy.top/gtogzpnbgu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgufenzy.top/gtymoyumqq.html

[Q68] 保存点
来源：http://hz.yvedp.cn/gtmqbcrkyg.html

SAVEPOINT sp1;
来源：http://hz.feifeiyinyue.top/gtbjrxqtxb.html

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtuuzirzbo.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtavkcvsrc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aibaodan.cn/gtooofsqkh.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtfdynhllu.html

ANALYZE TABLE users;
来源：http://hz.daxiang520.top/gtgnembaqy.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtbbmhnfoa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shuidangran.top/gtiddzkycs.html

[Q72] 查看索引
来源：http://hz.chenjidiqi.icu/gtqijtnikf.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gttmfmirms.html

[Q73] 查看表状态
来源：http://hz.vqdsnc.cn/gtogcsfrkb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinyuanbaomall.cn/gtntwjpcmh.html

[Q74] 强制使用索引
来源：http://hz.yj20258.top/gtxxoeyhfx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtwdtqlycj.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtbykxfbbu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cashguo.top/gtcvcijdoe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtjnestcct.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtpiatkkvq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cashguo.top/gtwlsssapw.html

[Q77] 时间加减
来源：http://hz.hysaishi.cn/gtjekulocc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yvedp.cn/gtvibdvsda.html

[Q78] 当前时间
来源：http://hz.yuxming.cn/gtggghtknd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nwbrower.top/gturnahurk.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtcjcdguxp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.bjfxy.top/gtkgeohimj.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtxwaodcfz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aizwys.cn/gtnfbebwsj.html

[Q81] 字符串替换
来源：http://hz.yongpay.top/gtxgwnkrrs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtwwjcszvo.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gthzqijgwa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuanzhike.top/gtyvksycwi.html

[Q83] 大小写转换
来源：http://hz.smart0.xyz/gtctpdnowi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtmjacysil.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtqpfcygkh.html

SELECT TRIM(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtuvijzrru.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtyanuiuii.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghu66.top/gtykubngzs.html

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtobursdoj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.iojbl.cn/gtreninmam.html

[Q87] JSON 字段做条件
来源：http://hz.zhengqikj.top/gthbysfzmj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xingfuxueyuan.xyz/gtteifsmro.html

[Q88] 行转列（条件聚合）
来源：http://hz.sysykeji.top/gtzndbrfkj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.svipenyu.cn/gtuxsosfvu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigfzy.top/gtfccfqvaq.html

[Q89] 判断表是否存在
来源：http://hz.tianlin.xyz/gtkahlwssm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gteqtdcpmq.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtwjmdbrnx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtwpdukibc.html

================================================================================
来源：http://hz.sxryk.cn/gtuudxkxou.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtjxokwzob.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmulymagc.html

[R01] shebang 与严格模式
来源：http://hz.hfpthk.cn/gtlhksyaty.html

#!/usr/bin/env bash
来源：http://hz.zhiwuduotai.top/gtjxppubav.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtuhoshtbs.html

[R02] 变量赋值与使用
来源：http://hz.yuanzhike.top/gtsjstgkid.html

name="Tom"; echo "$name"
来源：http://hz.fengsongda.top/gtpnfqntod.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtxvrjrvsp.html

readonly PI=3.14
来源：http://hz.tianlin.xyz/gtuvittfpc.html

[R04] 位置参数
来源：http://hz.andypj.xyz/gtvaxqovtf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shzxlz.cn/gtairwyykx.html

[R05] 参数默认值
来源：http://hz.ydzc1.top/gtehdjpyiy.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtystzlvyb.html

[R06] 判断命令是否存在
来源：http://hz.yj20258.top/gtaokrwojg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtczbhypkp.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtmytqochi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtkmzxvoho.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtqawygkps.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gtesggmytz.html

[R09] 字符串比较
来源：http://hz.cdnleiting.top/gtvztdtywc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gthzbeetmv.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtiwgjuvby.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ivvv.top/gtulxvbcnx.html

[R11] case 多分支
来源：http://hz.dashuyun.cn/gtqewkecld.html

case "$1" in
来源：http://hz.9152youxi.cn/gtyznfnhzw.html

start) echo "启动" ;;
来源：http://hz.yj202588.top/gtkrncwwpp.html

stop)  echo "停止" ;;
来源：http://hz.jlsjyb.cn/gtruycsglp.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtitpwlxgt.html

esac
来源：http://hz.chenzaomai.com/gtuijyhfkz.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gtpskhslhd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gtusfyjtjr.html

[R13] for 计数循环
来源：http://hz.guowangkeji.top/gtzjllbpke.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtksvpeatq.html

[R14] C 风格 for
来源：http://hz.vqdsnc.cn/gtoeaqkbsn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhengqikj.top/gtwzjvxghw.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtfzruoqdd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtmytbthuh.html

[R16] until 等待条件
来源：http://hz.chenzaomai.com/gtiofsgvdj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gttyzbnbkq.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gtkzxlxzjd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fengsongda.top/gthmkvrgni.html

[R18] 遍历数组
来源：http://hz.gaohongyu789.top/gtbdfvzeec.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtdasbktha.html

[R19] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtbufhpsvj.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtdqlmftfq.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtbsbulpyv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj202588.top/gtuknxehex.html

[R21] 字符串长度
来源：http://hz.xinyue.icu/gtrhshjmbz.html

echo "${#s}"
来源：http://hz.tianlin.xyz/gtbtkbkrlh.html

[R22] 截取子串
来源：http://hz.quarkkingdee.top/gtgwxczwrq.html

echo "${s:0:5}"
来源：http://hz.nwbrower.top/gtxicutbtg.html

[R23] 字符串替换
来源：http://hz.cucudq.cn/gttlltzxji.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtawlfezuz.html

[R24] 大小写转换
来源：http://hz.hnqzz.top/gtdnwljpok.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtijxyvgcw.html

[R25] 去后缀 / 去前缀
来源：http://hz.gaohongyu789.top/gtxzzdzxsv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tian-w.cn/gtljuewatm.html

[R26] 命令替换
来源：http://hz.yj202588.top/gtvwurfini.html

now=$(date +%F); echo "$now"
来源：http://hz.jinghuilouyu.cn/gtbgftvbxx.html

[R27] 算术展开
来源：http://hz.yuxming.cn/gtkxtdzwoq.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtpzowlxzf.html

[R28] 浮点运算
来源：http://hz.c1oappe.top/gtctyedtxd.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gtuzeymqef.html

[R29] 定义函数
来源：http://hz.gotoacloud.top/gtansnyqmi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtqsvgddcx.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtddrotkmk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fengsongda.top/gtmpewkahm.html

[R31] 局部变量
来源：http://hz.yj20258.top/gtisloelxj.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtzziuruhs.html

[R32] 参数个数校验
来源：http://hz.jyoumei.cn/gtgvchwutn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gaohongyu789.top/gtmaglvxnx.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtuqdimeuo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydjk.org.cn/gtevyjgnbj.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtmcoxpjhg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gtrldeefhw.html

[R35] 后台执行并等待
来源：http://hz.fzhhl.top/gtgyccagrn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gtrmuuiluq.html

[R36] 并发执行多个任务
来源：http://hz.nwbrower.top/gtvisswzmt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hongshengwenyu.top/gtpzcimysq.html

[R37] 把输出赋给变量
来源：http://hz.jinyuanbaomall.cn/gtukhjiunc.html

files=$(ls -1)
来源：http://hz.yj20258.top/gtjhzaagwr.html

[R38] 管道串联
来源：http://hz.birdmap.top/gthlcrcqwi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtkhznnvli.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtrrhppnfl.html

cmd > out.log 2>&1
来源：http://hz.nanxinkj.top/gtgoldzvxq.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtfhcevrvd.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtpyrvajcw.html

[R41] 丢弃输出
来源：http://hz.jqgufenzy.top/gtlqqzsylk.html

cmd >/dev/null 2>&1
来源：http://hz.jyoumei.cn/gtislvqewd.html

[R42] 输入重定向
来源：http://hz.zhongyouzk.top/gtcdhqnmdv.html

wc -l < a.txt
来源：http://hz.haohaochexian.top/gtgygjowis.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtakregwen.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtraqyytqc.html

[R44] 按修改时间查找
来源：http://hz.hfpthk.cn/gtiwuzltgp.html

find . -mtime -7 -type f
来源：http://hz.mhx1999.top/gtfvvjsbgk.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtzjdveuzv.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtjgcjzuhr.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtvzgipkvh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj202588.top/gttubqggfm.html

[R47] sed 单行替换
来源：http://hz.jianghu66.top/gtffntjdam.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtsanvkhgc.html

[R48] awk 取指定列
来源：http://hz.c1oappe.top/gtvljvdndo.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gtjxbtrkpj.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtascabnqi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhoulong.xyz/gtuquxmpll.html

[R50] awk 求和
来源：http://hz.zhongyouzk.top/gtqlvxspep.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenjidiqi.icu/gtgulmtwcf.html

[R51] 排序去重取前几
来源：http://hz.ydjk.org.cn/gthqfbiglk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenlongwang.top/gtemdixilo.html

[R52] 统计行数
来源：http://hz.tian-w.cn/gtblwuhxkw.html

wc -l a.txt
来源：http://hz.cdnleiting.top/gtlcpqgspr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtmzstixwe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zdqjudy.top/gthtaejuib.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gtrkfjoxbw.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtvmsdmack.html

[R55] 压缩与解压
来源：http://hz.nwbrower.top/gtnxevkbil.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gtppjjckab.html

[R56] 远程拷贝
来源：http://hz.iojbl.cn/gtyhzycjqg.html

scp file user@host:/path/
来源：http://hz.ivvv.top/gtpblsritm.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtczfpbxsw.html

ssh user@host 'uptime'
来源：http://hz.xylfe.cn/gtayryrkwh.html

[R58] 下载文件
来源：http://hz.daxiang520.top/gtiwxvfrxz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtcoqhslen.html

[R59] 发 POST JSON
来源：http://hz.hysaishi.cn/gtvmkgeymc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zycfv.cn/gtxbwobxly.html

[R60] 只看 HTTP 状态码
来源：http://hz.316326.xyz/gtptjirfxp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtiduyripy.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtejncnuel.html

df -h;  du -sh *
来源：http://hz.jinghuilouyu.cn/gtwnetvzii.html

[R62] 找最占空间的文件
来源：http://hz.meibo888.top/gtwoyflgdg.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtjkmdwrng.html

[R63] 内存与进程
来源：http://hz.zhixingplan.top/gtiuhrywrv.html

free -h;  ps aux | grep nginx
来源：http://hz.gzhubu.top/gtbuszvupm.html

[R64] 结束进程
来源：http://hz.tanke756.top/gteauegolk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gtpqxiobta.html

[R65] 查看端口占用
来源：http://hz.smart0.xyz/gtozglmjog.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhiwuduotai.top/gttadnsfei.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gthyyeueyi.html

crontab -e;  crontab -l
来源：http://hz.gaohongyu789.top/gtpskzoqei.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258.top/gtlmljlbtc.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtdryogbkv.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtmobzxngt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtpfrhbibo.html

[R69] 生成随机密码
来源：http://hz.havefunace.top/gtcukfzvyx.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtroxfedwy.html

[R70] 时间戳与互转
来源：http://hz.yuanzhike.top/gtoxwjvjgf.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigufen.top/gtpfthhbvp.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gtsjtcsngq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sufxvd.cn/gtlzjmbnba.html

[R72] 等待端口就绪
来源：http://hz.hywenlv.cn/gtiucycqzz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtcpmorgmn.html

[R73] 分割大日志
来源：http://hz.pengpengdd.cyou/gtsbqukqxb.html

split -l 1000 big.log part_
来源：http://hz.zhijiandao.cn/gtoivwelsk.html

[R74] 批量重命名
来源：http://hz.yj20258.top/gtqflpgien.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuanzhike.top/gtovvikaej.html

[R75] 导出环境变量
来源：http://hz.dashuyun.cn/gttszpcyya.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sweek.top/gtngvuzisy.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gteaqfpdsy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtdcgjoorv.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtcitzgqmj.html

read -rp "请输入: " ans
来源：http://hz.feifeiyinyue.top/gtvufkwloo.html

[R78] 交互式菜单
来源：http://hz.yanxiufei.cn/gtjugjtrzb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtiqmmdtil.html

[R79] 解析命令行选项
来源：http://hz.xinyue.icu/gtygxuisdi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gtxkxuumbs.html

[R80] 查看脚本执行耗时
来源：http://hz.hywenlv.cn/gtfvquefur.html

time ./run.sh
来源：http://hz.yj20258888.top/gtczuqlqcv.html

================================================================================
来源：http://hz.gogol.net.cn/gttpvrcibg.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtmnoezuca.html

================================================================================
来源：http://hz.nanxinkj.top/gtrnhvkbtk.html

[S01] C：Hello World
来源：http://hz.chenjidiqi.icu/gtswuybwag.html

#include <stdio.h>
来源：http://hz.zhengqikj.top/gtduyswrty.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hywenlv.cn/gtgdxunsbd.html

[S02] C：变量与格式化输出
来源：http://hz.wangshuangyany.cn/gtcxmrivvt.html

int a = 10; printf("%d\n", a);
来源：http://hz.meibo888.top/gtystodchh.html

[S03] C：读入整数
来源：http://hz.gogol.net.cn/gtqyteltjj.html

int x; scanf("%d", &x);
来源：http://hz.yvedp.cn/gtldeirlpw.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtouivyfth.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.andypj.xyz/gtqeneiklv.html

[S05] C：字符串长度
来源：http://hz.jinghuilouyu.cn/gttfwrorwv.html

strlen(s)
来源：http://hz.hfpthk.cn/gtxnjzquyk.html

[S06] C：字符串比较
来源：http://hz.kuanghao11.cn/gtjjbwtace.html

strcmp(a, b) == 0
来源：http://hz.gzhubu.top/gtlkcjkhgv.html

[S07] C：数组遍历求和
来源：http://hz.andypj.xyz/gtrwwiaxvh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgfzy.top/gtbrzzxxgn.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtvsjazfki.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtgjilmzqb.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtswcjhgla.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangkeji.top/gtfvjmlvrl.html

[S10] C：指针与解引用
来源：http://hz.tianlin.xyz/gtoltqexla.html

int *p = &a;  *p = 5;
来源：http://hz.52xcode.cn/gtsioviibu.html

[S11] C：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtistgwmyh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtlhineacx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtljaelwqr.html

fclose(f);
来源：http://hz.yj20258.top/gteqptvxun.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtkvbkmuad.html


<!-- 参考信息 -->