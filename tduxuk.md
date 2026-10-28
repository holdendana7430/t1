代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nwbrower.top/gtqahieujo.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtljubbwqz.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gtzqfqshlu.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigufen.top/gtmypbeidu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtkruumafc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtaydzpdds.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgufenzy.top/gtwpgnspjn.html

[Q57] 行号
来源：http://hz.guannengcc.top/gttafkdwig.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtzvvnryyk.html

[Q58] 累计求和
来源：http://hz.ybcxt.top/gtzvnusnnc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuanzhike.top/gthzywoxta.html

[Q59] 分组内累计
来源：http://hz.quarkkingdee.top/gtiqahudld.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gttkkwfiqe.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtwafebggk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtccczvcvj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gtsnxijuem.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gtzwbewvwe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtnpgnzteq.html

[Q62] 分组占比
来源：http://hz.daxiang520.top/gtoixxngqc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtlyxvtdzd.html

[Q63] 开启事务
来源：http://hz.sysykeji.top/gtzyhqxhjk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gtwwgjyubr.html

[Q64] 提交事务
来源：http://hz.tianlin.xyz/gtcsuhkdwm.html

COMMIT;
来源：http://hz.ehwqpu.com/gtubeoaiuz.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gtlnirhhgn.html

ROLLBACK;
来源：http://hz.gotoacloud.top/gtqgcivuxt.html

[Q66] 行锁查询
来源：http://hz.9152youxi.cn/gthaifvsdd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtwmrstlfz.html

[Q67] 设置隔离级别
来源：http://hz.ydzc1.top/gtosdorkhq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.smart0.xyz/gtomduujbj.html

[Q68] 保存点
来源：http://hz.sweek.top/gtxsggsqef.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtbdbpjeet.html

ROLLBACK TO sp1;
来源：http://hz.jyoumei.cn/gtrdqucvyq.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtoztdsxye.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gtiitseffn.html

[Q70] 更新统计信息
来源：http://hz.tianlin.xyz/gtjtbfuswh.html

ANALYZE TABLE users;
来源：http://hz.wangshuangyany.cn/gtqmoubick.html

[Q71] 查看建表语句
来源：http://hz.daria6918.cn/gtjllbjjvt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.iojbl.cn/gtevwkodho.html

[Q72] 查看索引
来源：http://hz.ppjwa.cn/gtggcoogut.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gttnmnnblh.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtnvqpcbhb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtuyovvtiq.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gtfjnqgbbq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangshuangyany.cn/gtklmzefsm.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtuyfogdgd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pengpengdd.cyou/gtiocbzfug.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sweek.top/gtrtxlvfjp.html

[Q76] 按天统计
来源：http://hz.shanyushiyangkeji.top/gteluajpgf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.redwolf501.top/gthnmhxhsu.html

[Q77] 时间加减
来源：http://hz.zycfv.cn/gtpplgemai.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtgtdqtmnn.html

[Q78] 当前时间
来源：http://hz.nanxuanxn.top/gtdqnnoewl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtxmrvhqya.html

[Q79] 字符串拼接
来源：http://hz.daria6918.cn/gtffhwmall.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sweek.top/gtqalgcxix.html

[Q80] 字符串截取
来源：http://hz.ppjwa.cn/gtvlobsobi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ppjwa.cn/gtamxgfcjs.html

[Q81] 字符串替换
来源：http://hz.cashguo.top/gtykrzhpnc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtmceypvox.html

[Q82] 字符长度与字节长度
来源：http://hz.xingfuxueyuan.xyz/gtmrkdibnj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hysaishi.cn/gtrjtebidq.html

[Q83] 大小写转换
来源：http://hz.jyoumei.cn/gtgxqsqbjh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtynzvtkhp.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtpejbfdgz.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtofknznic.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gtuzhxtmxs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtlqfoyzsw.html

[Q86] 读取 JSON 字段
来源：http://hz.cqqwz.cn/gtorpvbzoq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hywenlv.cn/gtrrhxeusw.html

[Q87] JSON 字段做条件
来源：http://hz.yongpay.top/gtndslkzna.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.9152youxi.cn/gtukemkorb.html

[Q88] 行转列（条件聚合）
来源：http://hz.gogol.net.cn/gtckmbuung.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.svipenyu.cn/gtjurzqnhr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jiagoushi.top/gtpkuzknqw.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtpkrggsql.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gtdxdnjwwq.html

[Q90] 生成序号列
来源：http://hz.jlsjyb.cn/gtlllfgmee.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.0kj1m.cn/gtkkmjnfnn.html

================================================================================
来源：http://hz.nanxinkj.top/gtbhnlvcmo.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtaszomqfs.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxhgdxvzn.html

[R01] shebang 与严格模式
来源：http://hz.gzhubu.top/gtzsnqasze.html

#!/usr/bin/env bash
来源：http://hz.shangyingyoupin.top/gtgplgvawo.html

set -euo pipefail
来源：http://hz.iojbl.cn/gtbonutdzv.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gtammyexnl.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtomipvebf.html

[R03] 只读变量
来源：http://hz.xziqi.cn/gtvlmdnguy.html

readonly PI=3.14
来源：http://hz.zhixingplan.top/gtrmsgizcc.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtgizwxkal.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hysaishi.cn/gtfcuqycil.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtzlwrwkfa.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtqzvffpmk.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtqsjjubio.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhengqikj.top/gtiyzfaknz.html

[R07] if 判断文件
来源：http://hz.zhoulong.xyz/gtqzxcwsda.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangkeji.top/gtvovddbtd.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gttjfhxujq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtnhoypunc.html

[R09] 字符串比较
来源：http://hz.pycfn.com/gtngbzxpth.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtbcionqja.html

[R10] 正则匹配
来源：http://hz.aibaodan.cn/gtklpmzpol.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtfzwfupuo.html

[R11] case 多分支
来源：http://hz.hfpthk.cn/gtdfimaysp.html

case "$1" in
来源：http://hz.yueranfly.top/gtoezjxlkm.html

start) echo "启动" ;;
来源：http://hz.xziqi.cn/gtkoywlhnl.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtycwkldqm.html

*)     echo "未知命令" ;;
来源：http://hz.ppjwa.cn/gtverdnyxe.html

esac
来源：http://hz.wangdashe.top/gtwodjovvl.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtyhdgfizh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gthumriuze.html

[R13] for 计数循环
来源：http://hz.wangshuangyany.cn/gtvrwyggyc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgfzy.top/gtuqnouvvd.html

[R14] C 风格 for
来源：http://hz.hnxiangtu.top/gtrvavfsuq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtkdoluijg.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtfejjjneg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnxiangtu.top/gtcypslldu.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtvwltwdtf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtogoqtyww.html

[R17] 数组定义与取值
来源：http://hz.xylfe.cn/gtrpotzplp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sweek.top/gtdklcjyqf.html

[R18] 遍历数组
来源：http://hz.smart0.xyz/gtrqpyjtfl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxuanxn.top/gttbdcqaen.html

[R19] 数组长度
来源：http://hz.mhx1999.top/gthtmkpajo.html

echo "${#arr[@]}"
来源：http://hz.hywenlv.cn/gtxyqaurqy.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtlmkxlwxi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtzgxjsifr.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtegaqiffy.html

echo "${#s}"
来源：http://hz.yj20258.top/gtjzigepyz.html

[R22] 截取子串
来源：http://hz.bjfxy.top/gteacyknnf.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtpyhlzjbj.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtmoockkdr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xylfe.cn/gtloubiauc.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtqnnbhpfs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gtxuxigper.html

[R25] 去后缀 / 去前缀
来源：http://hz.yvedp.cn/gtodveuofc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhoulong.xyz/gtwptlqqay.html

[R26] 命令替换
来源：http://hz.shangyingyoupin.top/gtmognkioq.html

now=$(date +%F); echo "$now"
来源：http://hz.daria6918.cn/gtvpsseoyo.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtjsjcyzel.html

echo $((1 + 2 * 3))
来源：http://hz.hnxiangtu.top/gtqllejjpi.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtnknmyquw.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gthymmavvc.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtocdfgvfc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dashuyun.cn/gtkcxdzejc.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtvkitzqfu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gtvgiepypg.html

[R31] 局部变量
来源：http://hz.yonumen.top/gtnezpmiud.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydzc1.top/gtvdoyphrg.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtnzeamidq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtywklewog.html

[R33] 捕获错误并提示行号
来源：http://hz.jlsjyb.cn/gtfhwenzje.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gzhubu.top/gtvdwjxwut.html

[R34] 退出时清理
来源：http://hz.jinyuanbaomall.cn/gthnmckbbx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtsfykxvkw.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtwxusayyg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtfyatppjk.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtkhvcypkd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hfpthk.cn/gtbwzbitcc.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtruutaegh.html

files=$(ls -1)
来源：http://hz.quarkkingdee.top/gtuoyrmsaz.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtbzudvbal.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gaohongyu789.top/gtvhxhcvij.html

[R39] 重定向标准输出与错误
来源：http://hz.quarkkingdee.top/gtxlajitat.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gtxmstrcnx.html

[R40] 追加写日志
来源：http://hz.hnqzz.top/gtvllilrzv.html

echo "log" >> out.log
来源：http://hz.jiagoushi.top/gtcaznczvd.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtvkkkvbii.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtriyaofna.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtfdoganpm.html

wc -l < a.txt
来源：http://hz.yueranfly.top/gtorfwucrt.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gtzkfsvpzn.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtdkanonqq.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtljaxqhtn.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtiaujvlgq.html

[R45] 批量删除
来源：http://hz.feifeiyinyue.top/gtzadrhoaj.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtrlidhazq.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtpaxfynrv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tanke756.top/gtuzwmpbro.html

[R47] sed 单行替换
来源：http://hz.yj20258888.top/gtpgmcyssf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tianlin.xyz/gtusziqjtz.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtgiquzjwx.html

awk '{print $1, $3}' a.txt
来源：http://hz.feifeiyinyue.top/gtokfpvcta.html

[R49] awk 带条件
来源：http://hz.snrcjt.cn/gtkacvvhkl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtbcwstrmp.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtporgrcsn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtokdpwawq.html

[R51] 排序去重取前几
来源：http://hz.svipenyu.cn/gtztqxfweu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gtcrothcid.html

[R52] 统计行数
来源：http://hz.shangyingyoupin.top/gtwuskzicz.html

wc -l a.txt
来源：http://hz.shanyushiyangtech.top/gtghtvvxhr.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtfkhhpaxb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtnttrxzqq.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtirmezdls.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtshohcagl.html

[R55] 压缩与解压
来源：http://hz.sysykeji.top/gtivltewax.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.316326.xyz/gtmkdybusb.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtvdzsqluw.html

scp file user@host:/path/
来源：http://hz.zdqjudy.top/gtnawgtdth.html

[R57] 远程执行命令
来源：http://hz.wangdashe.top/gtgondcqwl.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtmnyixpvx.html

[R58] 下载文件
来源：http://hz.jqgfzy.top/gtmwaockcq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtpdlgdcrx.html

[R59] 发 POST JSON
来源：http://hz.fzhhl.top/gtocaaisni.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtquwlugxe.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtydcjdlrr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtomaajqqo.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtxeihghha.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtlcevtsui.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtntbvilrr.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gtpzfyhbse.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtnbitwtnu.html

free -h;  ps aux | grep nginx
来源：http://hz.jinghuilouyu.cn/gtbangslbe.html

[R64] 结束进程
来源：http://hz.cucudq.cn/gtahmdfobj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sxryk.cn/gtebooyows.html

[R65] 查看端口占用
来源：http://hz.svipenyu.cn/gtjtxhbyma.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.0kj1m.cn/gtucowzzix.html

[R66] 定时任务
来源：http://hz.sweek.top/gtnouvawpt.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangkeji.top/gtamiaqmpn.html

[R67] 生成随机十六进制串
来源：http://hz.yuxming.cn/gtchkzyxnv.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtypscwoig.html

[R68] 计算文件校验值
来源：http://hz.bjfxy.top/gtojghoehl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.svipenyu.cn/gtxnfpkdki.html

[R69] 生成随机密码
来源：http://hz.c1oappe.top/gtabbstirt.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgfzy.top/gtktygrgmf.html

[R70] 时间戳与互转
来源：http://hz.meibo888.top/gtlgobdnyr.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtmzhniukb.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtkhqquekb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cashguo.top/gtnvxpyjza.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtpfbtomgw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gtbfihstxd.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gtjgrumkuu.html

split -l 1000 big.log part_
来源：http://hz.sweek.top/gtxeykaaxr.html

[R74] 批量重命名
来源：http://hz.cdnleiting.top/gtkzlbhzzw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigufen.top/gtvekriofk.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtzllndlff.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtnynnbolm.html

[R76] 使用临时文件
来源：http://hz.cucudq.cn/gtuhfzlnhp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtlcbdxvwy.html

[R77] 读取用户输入
来源：http://hz.xylfe.cn/gtzzgiybjd.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtgxdduikv.html

[R78] 交互式菜单
来源：http://hz.sysykeji.top/gtcuvbiohr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cheryme.top/gtnntspwtd.html

[R79] 解析命令行选项
来源：http://hz.jqgfzy.top/gtffdbokrw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtczutzzfd.html

[R80] 查看脚本执行耗时
来源：http://hz.zhengqikj.top/gtppoxmmgd.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtngvvpwof.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtixiicnge.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtprmusdgo.html

================================================================================
来源：http://hz.jiagoushi.top/gtdwhhlbjb.html

[S01] C：Hello World
来源：http://hz.nanxinkj.top/gtrqigmxrm.html

#include <stdio.h>
来源：http://hz.yongpay.top/gtoospjuuq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xylfe.cn/gtjtuybrvu.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtjpeoiluw.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtstluunas.html

[S03] C：读入整数
来源：http://hz.shzxlz.cn/gteceuzdwo.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtjjthuslk.html

[S04] C：字符串复制
来源：http://hz.zhaomingkeji.xyz/gtuqekqdmq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenlongwang.top/gtweovaoqk.html

[S05] C：字符串长度
来源：http://hz.sxryk.cn/gtphidanrm.html

strlen(s)
来源：http://hz.jinqigfzy.top/gtjgdddzxj.html

[S06] C：字符串比较
来源：http://hz.yj202588.top/gtrfkaaxmb.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtjxjxskxb.html

[S07] C：数组遍历求和
来源：http://hz.nanxinkj.top/gtxxgcpiiu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.svipenyu.cn/gtkftixrag.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtjkazerny.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sweek.top/gtcdnxzdkq.html

[S09] C：结构体定义与初始化
来源：http://hz.zhixingplan.top/gtlyeibrct.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.feifeiyinyue.top/gtntcfjule.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtskfkgbsf.html

int *p = &a;  *p = 5;
来源：http://hz.yuanzhike.top/gtjbapeoqt.html

[S11] C：逐行读文件
来源：http://hz.pengpengdd.cyou/gtqodriqli.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.meibo888.top/gtlwxuhmbl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.quarkkingdee.top/gtjtfmtquf.html

fclose(f);
来源：http://hz.svipenyu.cn/gtoyggnjcw.html

[S12] C：写文件
来源：http://hz.cdnleiting.top/gtggornkqe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtqqbrtvah.html

[S13] C：宏定义
来源：http://hz.jinyuanbaomall.cn/gtwhwwandu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hfpthk.cn/gtmubohymx.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gteytcrnhl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtnztzfacz.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtbikqwtlr.html

(double) a / b
来源：http://hz.havefunace.top/gtqjiwhqfm.html

[S16] C：位操作置位
来源：http://hz.zycfv.cn/gtadutxztj.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtmdefdjir.html

[S17] C：安全拼接字符串
来源：http://hz.sysykeji.top/gtyxeejcti.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtciznzsig.html

[S18] C：命令行参数
来源：http://hz.zhiwuduotai.top/gtqbnpyqkg.html

int main(int argc, char **argv)
来源：http://hz.sxryk.cn/gtltfdoaud.html

[S19] C：快速排序
来源：http://hz.pycfn.com/gtwykrryfu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtkmykbehj.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gttbsyyfvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gttkvcjbdw.html

[S21] C：字符类别判断
来源：http://hz.hongshengwenyu.top/gtevcoscct.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.meibo888.top/gtjfpdrzer.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gtqmfpsvue.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtpuegscfs.html

[S23] C：随机数
来源：http://hz.shuidangran.top/gtvmsgijkd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ivvv.top/gtndopyxdl.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtellzubwq.html


<!-- 参考信息 -->