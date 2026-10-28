代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtqcghltff.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtjbtacwzm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtszjsuryb.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtmhqweuin.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtbclahqdr.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxuanxn.top/gtldzywxpk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtybyulctg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gtbciuhqec.html

[Q61] 移动平均
来源：http://hz.gaohongyu789.top/gtrdgrbctt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.vqdsnc.cn/gtmxthvcbz.html

[Q62] 分组占比
来源：http://hz.316326.xyz/gtdbhdesby.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtnbnqchfu.html

[Q63] 开启事务
来源：http://hz.shangyingyoupin.top/gtanqzejhs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.smart0.xyz/gtjoirodwv.html

[Q64] 提交事务
来源：http://hz.redwolf501.top/gtyyhmztwg.html

COMMIT;
来源：http://hz.pengpengdd.cyou/gthfbzjouz.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtvwryfdsm.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtytysgjqc.html

[Q66] 行锁查询
来源：http://hz.yueranfly.top/gtszafgksq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhixingplan.top/gtbvnlmfeg.html

[Q67] 设置隔离级别
来源：http://hz.vqdsnc.cn/gtiariutai.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aizwys.cn/gtkszfjsdu.html

[Q68] 保存点
来源：http://hz.hnqzz.top/gtagjlyzak.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gtcfddulas.html

ROLLBACK TO sp1;
来源：http://hz.jinghuilouyu.cn/gtprldmdwx.html

[Q69] 查看执行计划
来源：http://hz.tian-w.cn/gtorcosxez.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pycfn.com/gtqvjdbtsx.html

[Q70] 更新统计信息
来源：http://hz.jinqigufen.top/gtrcfihrzz.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtbvjuzmpq.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtpugkmjpr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yvedp.cn/gtgsildaaj.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gtribyozdb.html

SHOW INDEX FROM users;
来源：http://hz.shanyushiyangtech.top/gtvregtyhp.html

[Q73] 查看表状态
来源：http://hz.gzhubu.top/gtduqycxpl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sweek.top/gtmrjioubi.html

[Q74] 强制使用索引
来源：http://hz.andypj.xyz/gtdxiyyjss.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtssjeatqj.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtqlhcneqw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sweek.top/gtewbhlpyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xuetiantiany.cn/gtlqjtabee.html

[Q76] 按天统计
来源：http://hz.gotoacloud.top/gtctctljad.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guowangkeji.top/gtvtpexvet.html

[Q77] 时间加减
来源：http://hz.cdnleiting.top/gtlnqlwedw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtwqiesjoh.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtxfawcypf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.meibo888.top/gtgjsmzwpo.html

[Q79] 字符串拼接
来源：http://hz.cucudq.cn/gtmytxrzbr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtwezsewiw.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangkeji.top/gtetzyifdk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zdqjudy.top/gtavtvzpij.html

[Q81] 字符串替换
来源：http://hz.svipenyu.cn/gtktpbrntv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cheryme.top/gttnuphnsg.html

[Q82] 字符长度与字节长度
来源：http://hz.xylfe.cn/gtyxxuqrno.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtetwyglch.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtozpzsrzv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtepvinbhf.html

[Q84] 去除首尾空格
来源：http://hz.guannengcc.top/gtgcikmcgd.html

SELECT TRIM(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtyyyxmzox.html

[Q85] 数值取整
来源：http://hz.redwolf501.top/gtjsbxvmlx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258.top/gtmdrzsgjs.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtqeoqngzo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ivvv.top/gtumaneawv.html

[Q87] JSON 字段做条件
来源：http://hz.zdqjudy.top/gtueiknumz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gtytyfcosv.html

[Q88] 行转列（条件聚合）
来源：http://hz.ivvv.top/gtkcapycdg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hywenlv.cn/gthofnpsve.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zdqjudy.top/gtinowacbz.html

[Q89] 判断表是否存在
来源：http://hz.tian-w.cn/gtvchzdtrf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtrocoakyd.html

[Q90] 生成序号列
来源：http://hz.zhaomingkeji.xyz/gtzwajzhnb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtufjnhgzy.html

================================================================================
来源：http://hz.tanke756.top/gtkssxelmm.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtbtfwqitx.html

================================================================================
来源：http://hz.fengsongda.top/gtlahfllhh.html

[R01] shebang 与严格模式
来源：http://hz.daxiang520.top/gttmjmlylg.html

#!/usr/bin/env bash
来源：http://hz.yuxming.cn/gthaaxchzp.html

set -euo pipefail
来源：http://hz.ydjk.org.cn/gtqqxulclc.html

[R02] 变量赋值与使用
来源：http://hz.zhiwuduotai.top/gtqoqesdig.html

name="Tom"; echo "$name"
来源：http://hz.guowangkeji.top/gtiwnurnea.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtpeyrwbqm.html

readonly PI=3.14
来源：http://hz.birdmap.top/gtypmbnbdu.html

[R04] 位置参数
来源：http://hz.quarkkingdee.top/gtpjujnlgu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigufen.top/gtmxtdzftq.html

[R05] 参数默认值
来源：http://hz.daxiang520.top/gtmcvryqcf.html

name="${1:-default}"
来源：http://hz.andypj.xyz/gttzhuqqay.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtuaxtzpts.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtsrzkyndg.html

[R07] if 判断文件
来源：http://hz.shuidangran.top/gtqkrkpapk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.vqdsnc.cn/gtathvcmsi.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtxkxraqyo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtowfqhhfs.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtgsasqyjm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.havefunace.top/gtnlxdjqiy.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gtgognthwm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gthicelmky.html

[R11] case 多分支
来源：http://hz.shanyushiyangkeji.top/gtortqwbnb.html

case "$1" in
来源：http://hz.shuidangran.top/gtoizextxf.html

start) echo "启动" ;;
来源：http://hz.jianghu66.top/gtghahxshs.html

stop)  echo "停止" ;;
来源：http://hz.dashuyun.cn/gtufdygugz.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangtech.top/gtnakshhky.html

esac
来源：http://hz.jinqigufen.top/gtgjsxvobw.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtatnugkeh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xinyue.icu/gtsorpuqlf.html

[R13] for 计数循环
来源：http://hz.wangdashe.top/gtsfmadtst.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtrkjmjnce.html

[R14] C 风格 for
来源：http://hz.zhaomingkeji.xyz/gtkliysqpw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gotoacloud.top/gtkbfllfrv.html

[R15] while 逐行读文件
来源：http://hz.zhengqikj.top/gtjpgxvwjb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jlsjyb.cn/gtvseahvxe.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtwxsvkktc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtxkmsvhvu.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtwffusquz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gtmottofmw.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtyvymbsoo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhijiandao.cn/gtefipmvyg.html

[R19] 数组长度
来源：http://hz.hongshengwenyu.top/gtqdvyxqxs.html

echo "${#arr[@]}"
来源：http://hz.andypj.xyz/gtrmmtnxcw.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtwkyygiqs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtxkylnhbf.html

[R21] 字符串长度
来源：http://hz.gotoacloud.top/gtxmswzxju.html

echo "${#s}"
来源：http://hz.xingfuxueyuan.xyz/gteurgaauc.html

[R22] 截取子串
来源：http://hz.fzhhl.top/gtngnuheye.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtgmjiowgr.html

[R23] 字符串替换
来源：http://hz.pengpengdd.cyou/gtkjaikwbj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtpiwgvist.html

[R24] 大小写转换
来源：http://hz.svipenyu.cn/gtpqgvjqho.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhijiandao.cn/gtmgrwuxdf.html

[R25] 去后缀 / 去前缀
来源：http://hz.yangfankeji.com/gtwdomdhgx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gtipndodca.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gtxigepcrf.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gteliuwdjf.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtfkwfjagg.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtdjcgxcjq.html

[R28] 浮点运算
来源：http://hz.zhijiandao.cn/gtzctqortx.html

echo "scale=2; 10/3" | bc
来源：http://hz.mhx1999.top/gtqdludzdc.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtmliwcdif.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtzznrsvkd.html

[R30] 函数返回状态码
来源：http://hz.snrcjt.cn/gtqdugiqrp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtttcwpfim.html

[R31] 局部变量
来源：http://hz.ydzc1.top/gtvvdshyqm.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtrgkryjal.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtbdybyelw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtlznxclrt.html

[R33] 捕获错误并提示行号
来源：http://hz.zhaomingkeji.xyz/gtqvfnlake.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.316326.xyz/gtfhmzytlf.html

[R34] 退出时清理
来源：http://hz.9152youxi.cn/gtuepgozmi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtzglpopoj.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtwqlwpauj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtfxznyptl.html

[R36] 并发执行多个任务
来源：http://hz.gzhubu.top/gtbzwelthn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtmvyjlyoh.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtfqajpvaa.html

files=$(ls -1)
来源：http://hz.xuetiantiany.cn/gtzlxodtok.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtwjxvwjgw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.316326.xyz/gtudnbefzd.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtaxjypndi.html

cmd > out.log 2>&1
来源：http://hz.ivvv.top/gtuhvbitym.html

[R40] 追加写日志
来源：http://hz.xziqi.cn/gtuzndnhyc.html

echo "log" >> out.log
来源：http://hz.gaohongyu789.top/gtgnnhuxce.html

[R41] 丢弃输出
来源：http://hz.zycfv.cn/gtosucvoke.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gtgxuktafj.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtynhdsdyd.html

wc -l < a.txt
来源：http://hz.yangfankeji.com/gtgqfiocft.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gttbjylijv.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtauaudzwg.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtabvrkamh.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gtayckapey.html

[R45] 批量删除
来源：http://hz.tianlin.xyz/gtoiilsojg.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtzkloljia.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gtkcpzfycq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xingfuxueyuan.xyz/gtpiyqzthd.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtzgtdthio.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtzllrwobf.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtiumamqvk.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhiwuduotai.top/gtqnnetkwg.html

[R49] awk 带条件
来源：http://hz.ivvv.top/gtwjlydaqv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yangfankeji.com/gtuajhnciv.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtaczlfyil.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj202588.top/gtqepowzqb.html

[R51] 排序去重取前几
来源：http://hz.chenjidiqi.icu/gtblucflcr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gtmbotdqsu.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtvnrrsyhs.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtimfvwfpo.html

[R53] 查看文件头与实时尾
来源：http://hz.vqdsnc.cn/gtorzvwrta.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydjk.org.cn/gthsvyopyr.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gtqscurktn.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtfquhdjme.html

[R55] 压缩与解压
来源：http://hz.birdmap.top/gtfmftiisz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtdpftowzp.html

[R56] 远程拷贝
来源：http://hz.kuanghao11.cn/gtpuyoemwr.html

scp file user@host:/path/
来源：http://hz.yvedp.cn/gtntntwojq.html

[R57] 远程执行命令
来源：http://hz.daxiang520.top/gtwmzpgtzt.html

ssh user@host 'uptime'
来源：http://hz.pengpengdd.cyou/gtygzapobj.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtqcphdhfj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtxtxoqepv.html

[R59] 发 POST JSON
来源：http://hz.jyoumei.cn/gtyviwvtdg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cucudq.cn/gtxczgnvie.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtwyreydol.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gttgwvrnjj.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gtcwhnlgxb.html

df -h;  du -sh *
来源：http://hz.jlsjyb.cn/gtuyfqlqgh.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtlhfinivf.html

du -ah . | sort -rh | head -10
来源：http://hz.cheryme.top/gtngvdhbgu.html

[R63] 内存与进程
来源：http://hz.iojbl.cn/gtbeyjppxr.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtmokebolb.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtriowajpj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhoulong.xyz/gtxhdhawvu.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtgrdjvunt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtkuwifrzc.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtbqpaxxsg.html

crontab -e;  crontab -l
来源：http://hz.snrcjt.cn/gtrvcyqcrz.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gtzhyivytp.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtmurrzwnh.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gtmgyenfms.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gthtzbgkjn.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gtqmqkiqdn.html

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gtyddzoahe.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtgvrangon.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gtkvtfxxtd.html

[R71] 日期格式化
来源：http://hz.dianchejie.cn/gtdnhjmbkf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fzhhl.top/gtngwqcnqs.html

[R72] 等待端口就绪
来源：http://hz.birdmap.top/gtdfptxqsv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtueqemamw.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gtmrusiixg.html

split -l 1000 big.log part_
来源：http://hz.yonumen.top/gtvajxkamj.html

[R74] 批量重命名
来源：http://hz.xuetiantiany.cn/gtozemedgg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dianchejie.cn/gtdoujmyvu.html

[R75] 导出环境变量
来源：http://hz.hnqzz.top/gtujgopckd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtdpqrasau.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtakvmmgku.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtexgfwnsu.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtyzphibql.html

read -rp "请输入: " ans
来源：http://hz.yongpay.top/gtzieocwdu.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtmwktfkdf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pengpengdd.cyou/gtxpiufytv.html

[R79] 解析命令行选项
来源：http://hz.fzhhl.top/gtdvfruwcu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jlsjyb.cn/gtsslsiqvq.html

[R80] 查看脚本执行耗时
来源：http://hz.cucudq.cn/gttngdhraj.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtnnbesijw.html

================================================================================
来源：http://hz.tianlin.xyz/gtvruqogay.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gtkzngsxsf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrdolljff.html

[S01] C：Hello World
来源：http://hz.gotoacloud.top/gttfnbhjqu.html

#include <stdio.h>
来源：http://hz.cucudq.cn/gtchhezcyo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shzxlz.cn/gtythitesn.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtbgchjctd.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtucanemaz.html

[S03] C：读入整数
来源：http://hz.pycfn.com/gtqprobkdq.html

int x; scanf("%d", &x);
来源：http://hz.hnqzz.top/gtkeaqrhgv.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtxhunqgey.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenlongwang.top/gtccdxuxws.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gtzymplqhy.html

strlen(s)
来源：http://hz.quarkkingdee.top/gtvuajdznd.html

[S06] C：字符串比较
来源：http://hz.daria6918.cn/gtcmxxbzad.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtdqabiqhj.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtxwcjrksq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.svipenyu.cn/gtabrdujiv.html

[S08] C：动态内存分配与释放
来源：http://hz.hywenlv.cn/gtuejljymx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangtech.top/gtlhepyqmh.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gtxngjuory.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtcodvavnj.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtpozqsovc.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gtnopqekrv.html

[S11] C：逐行读文件
来源：http://hz.shzxlz.cn/gtjhyhorvp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daria6918.cn/gthgmsjlie.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.316326.xyz/gttaoxgrnb.html

fclose(f);
来源：http://hz.yj202588.top/gtijiaryby.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtxjjlytmg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtffdlzmas.html

[S13] C：宏定义
来源：http://hz.hysaishi.cn/gtgmzwqyzb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.birdmap.top/gtslwucutq.html

[S14] C：枚举
来源：http://hz.yuxming.cn/gtohpncirf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.c1oappe.top/gtmaksmzik.html

[S15] C：类型转换
来源：http://hz.yanxiufei.cn/gtmacvnyge.html

(double) a / b
来源：http://hz.sufxvd.cn/gtcrvvwvhl.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtnlrlmthu.html

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtjdufftwh.html

[S17] C：安全拼接字符串
来源：http://hz.sufxvd.cn/gtpyrvudxm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gtoknhnwta.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtftfqxfrh.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtbvypxwis.html

[S19] C：快速排序
来源：http://hz.yonumen.top/gtmtzezsnu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtyuktwujp.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtkuijitlr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtvywqqmps.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtvsdtgeez.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtctqgbycn.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtxuyfqkdz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtwgdvpsit.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gteqwbfyao.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cucudq.cn/gtbqennqya.html

[S24] C：获取本地时间
来源：http://hz.nanxuanxn.top/gturbqnzux.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zycfv.cn/gtbkzouxtt.html

[S25] C：内存拷贝
来源：http://hz.smart0.xyz/gtshhsoyfu.html

memcpy(dst, src, n);
来源：http://hz.dianchejie.cn/gteuoovhzi.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtivnecrsw.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtgkovfeyg.html

[S27] C：定义常量
来源：http://hz.yongpay.top/gtztcpyxns.html

const double PI = 3.14159;
来源：http://hz.wangdashe.top/gtppaoazcu.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtdbtulkgd.html


<!-- 参考信息 -->