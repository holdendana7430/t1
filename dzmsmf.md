代发 wailian999

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtyeaudsjr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cashguo.top/gtzgztehcz.html

[Q62] 分组占比
来源：http://hz.hnxiangtu.top/gtbfgchkha.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtknwifcrp.html

[Q63] 开启事务
来源：http://hz.fzhhl.top/gtewyvvdih.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guannengcc.top/gtnpcumjex.html

[Q64] 提交事务
来源：http://hz.fengsongda.top/gtadwbcqca.html

COMMIT;
来源：http://hz.iojbl.cn/gtddtjqbyc.html

[Q65] 回滚事务
来源：http://hz.yvedp.cn/gtwkzgsxar.html

ROLLBACK;
来源：http://hz.hysaishi.cn/gtwzqqykeq.html

[Q66] 行锁查询
来源：http://hz.dashuyun.cn/gtndgxfeey.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.iojbl.cn/gtnppnalbp.html

[Q67] 设置隔离级别
来源：http://hz.tanke756.top/gtkrpcwuch.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtanosocyu.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtcyoprcjs.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtrbvpgbzl.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtotsnymtm.html

[Q69] 查看执行计划
来源：http://hz.chenzaomai.com/gtkymmqdwh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtjfvzryft.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtgiauuuap.html

ANALYZE TABLE users;
来源：http://hz.redwolf501.top/gtsnttyaly.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gtokokpfnc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtrrdrotzl.html

[Q72] 查看索引
来源：http://hz.iojbl.cn/gtlimdlwzh.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gthpznkxji.html

[Q73] 查看表状态
来源：http://hz.jqgufenzy.top/gticojdtuv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydzc1.top/gttyjisgcw.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtxguwzubz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ybcxt.top/gthlfxhnps.html

[Q75] 日期格式化
来源：http://hz.quarkkingdee.top/gtgmssgtsi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gtdllklrjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sysykeji.top/gtpjzmyntj.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gttomtiywf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ehwqpu.com/gtctcseonq.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gtywprajia.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtrxsirgsi.html

[Q78] 当前时间
来源：http://hz.gogol.net.cn/gtehjsrkxg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtqnknxyxm.html

[Q79] 字符串拼接
来源：http://hz.cucudq.cn/gtfiwmpkaz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.iojbl.cn/gtecfbqsog.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtxvfiigvw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtiapmeyqy.html

[Q81] 字符串替换
来源：http://hz.guowangkeji.top/gtpnadqzhz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shangyingyoupin.top/gtndtgxwin.html

[Q82] 字符长度与字节长度
来源：http://hz.iojbl.cn/gtqdctglzn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtazbbkjqg.html

[Q83] 大小写转换
来源：http://hz.xylfe.cn/gteonqieoe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tianlin.xyz/gtklztupcb.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gtmwdbnqzr.html

SELECT TRIM(name) FROM users;
来源：http://hz.tianlin.xyz/gtxcpfxvft.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gttoivqfkk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gthqlzazcj.html

[Q86] 读取 JSON 字段
来源：http://hz.0kj1m.cn/gtontffkbp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnqzz.top/gtepbzqwxp.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtzkjvbmug.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gtqyalajcy.html

[Q88] 行转列（条件聚合）
来源：http://hz.fzhhl.top/gtzjpgndmk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtljguimlr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jyoumei.cn/gtfnczequl.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gtzhzgioyc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.iojbl.cn/gtjjeasthe.html

[Q90] 生成序号列
来源：http://hz.yj202588.top/gtcmesoape.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jlsjyb.cn/gtaydysfmp.html

================================================================================
来源：http://hz.smart0.xyz/gtzakgxgsl.html

R. Bash 专题
来源：http://hz.ivvv.top/gtofukyytk.html

================================================================================
来源：http://hz.guowangkeji.top/gthfrhtvgh.html

[R01] shebang 与严格模式
来源：http://hz.yueranfly.top/gthvprimbz.html

#!/usr/bin/env bash
来源：http://hz.yanxiufei.cn/gttepyxusw.html

set -euo pipefail
来源：http://hz.yueranfly.top/gtyadbueam.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtxivogskf.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gtjznjzedr.html

[R03] 只读变量
来源：http://hz.chenzaomai.com/gtsnnrmwqk.html

readonly PI=3.14
来源：http://hz.cheryme.top/gtgqhirbgc.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtgatykvxg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtffhbraou.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtlnrowyqj.html

name="${1:-default}"
来源：http://hz.pengpengdd.cyou/gtaitcozpc.html

[R06] 判断命令是否存在
来源：http://hz.hammf.cn/gtvjyrscdh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhijiandao.cn/gtbgregakz.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtftmrpykn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtvjgfbtlj.html

[R08] 数值比较
来源：http://hz.yj20258.top/gtkeynomjz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gtzbcdntbm.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtlcemljmo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtqihflwas.html

[R10] 正则匹配
来源：http://hz.nwbrower.top/gtgkywhxez.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhengqikj.top/gtqkpahufa.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gtyazrdiwg.html

case "$1" in
来源：http://hz.gogol.net.cn/gthgxpuuvr.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtsaxnncjs.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gtskxtuyer.html

*)     echo "未知命令" ;;
来源：http://hz.yonumen.top/gtvmmsirhu.html

esac
来源：http://hz.c1oappe.top/gtsjmvwumm.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtobkxiaww.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtqlzeczxy.html

[R13] for 计数循环
来源：http://hz.ybcxt.top/gtkwxejgll.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.meibo888.top/gtucsmgmkn.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gtdljrljuq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtxxlgxebm.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gtcggbvnzo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gogol.net.cn/gtpwkecwvl.html

[R16] until 等待条件
来源：http://hz.yonumen.top/gtjhdmpzzh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtvloxhvoi.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtkgqcveez.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gzhubu.top/gtodzuzpyl.html

[R18] 遍历数组
来源：http://hz.iojbl.cn/gtojqtsnel.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cheryme.top/gtysbmtdak.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtpdonvkbq.html

echo "${#arr[@]}"
来源：http://hz.yonumen.top/gterpfmted.html

[R20] 关联数组（字典）
来源：http://hz.52xcode.cn/gtlblpxjmt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pengpengdd.cyou/gtqnevytxx.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtnoijwerq.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtaswloccl.html

[R22] 截取子串
来源：http://hz.zdqjudy.top/gthogijkmk.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtvxmkprbv.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gthjfedpfd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtanftriqo.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtiadgoomw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.iojbl.cn/gtuupqlrhh.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258888.top/gtwgzcnyll.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gtgkpsfbzq.html

[R26] 命令替换
来源：http://hz.birdmap.top/gtygywwnnm.html

now=$(date +%F); echo "$now"
来源：http://hz.hnxiangtu.top/gtlhswfqnj.html

[R27] 算术展开
来源：http://hz.yuxming.cn/gtdaqbylqq.html

echo $((1 + 2 * 3))
来源：http://hz.hongshengwenyu.top/gthlhcpmam.html

[R28] 浮点运算
来源：http://hz.haohaochexian.top/gtpwkoyvsl.html

echo "scale=2; 10/3" | bc
来源：http://hz.guannengcc.top/gtqlinkdxg.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gtypcqxkqn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gtlxaeketv.html

[R30] 函数返回状态码
来源：http://hz.cashguo.top/gteibbzgkr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtexsnhups.html

[R31] 局部变量
来源：http://hz.aizwys.cn/gtugunihgs.html

f() { local x=1; echo "$x"; }
来源：http://hz.cashguo.top/gtwswnqxzm.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gtaanoveup.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gotoacloud.top/gtayoweuyl.html

[R33] 捕获错误并提示行号
来源：http://hz.xziqi.cn/gtwfgsbhuq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtpwnrobls.html

[R34] 退出时清理
来源：http://hz.zhaomingkeji.xyz/gtkjdtodqj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtkflyaouc.html

[R35] 后台执行并等待
来源：http://hz.nwbrower.top/gtcebjumma.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gotoacloud.top/gtkchwebvk.html

[R36] 并发执行多个任务
来源：http://hz.sysykeji.top/gtnsuxuapu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gthiwnpcsf.html

[R37] 把输出赋给变量
来源：http://hz.yuxming.cn/gtzhqyxmcz.html

files=$(ls -1)
来源：http://hz.sxryk.cn/gtvzvtwtrw.html

[R38] 管道串联
来源：http://hz.chenlongwang.top/gtsznrxwdc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtchnykmhw.html

[R39] 重定向标准输出与错误
来源：http://hz.0kj1m.cn/gtrihfoivz.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtjahplilm.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtnykfyjwc.html

echo "log" >> out.log
来源：http://hz.gogol.net.cn/gtbuugxqsk.html

[R41] 丢弃输出
来源：http://hz.vqdsnc.cn/gtadaqtlbb.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gthokjjbuh.html

[R42] 输入重定向
来源：http://hz.jlsjyb.cn/gtmfkiaqix.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtvvwsdskz.html

[R43] 按名字查找文件
来源：http://hz.zdqjudy.top/gttdgvmszq.html

find . -name "*.log" -type f
来源：http://hz.yuanzhike.top/gtkgcuomps.html

[R44] 按修改时间查找
来源：http://hz.ivvv.top/gtfnyfwjiq.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gtmrdknkxk.html

[R45] 批量删除
来源：http://hz.zycfv.cn/gtujtfuyhk.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gtrkludojv.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtafsbyqkm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.haohaochexian.top/gthvfvovli.html

[R47] sed 单行替换
来源：http://hz.vqdsnc.cn/gtxzhxxlqv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtfqpmygrv.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtpmndlaao.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gttameezsh.html

[R49] awk 带条件
来源：http://hz.aizwys.cn/gtsmiatnuu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinqigufen.top/gtzwopinmx.html

[R50] awk 求和
来源：http://hz.feifeiyinyue.top/gtabpnfbvd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gtzdvfzbie.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtutpldsdq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtxzvekqlf.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtyhzucwxc.html

wc -l a.txt
来源：http://hz.jiagoushi.top/gtthwhuidb.html

[R53] 查看文件头与实时尾
来源：http://hz.shangyingyoupin.top/gtnzqletnu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.9152youxi.cn/gtpxfmbplg.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtuervqzap.html

diff a.txt b.txt
来源：http://hz.c1oappe.top/gtdhhcetqp.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtqekdkvem.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtfrqkvtrx.html

[R56] 远程拷贝
来源：http://hz.yj20258888.top/gttisesres.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtfdglsfux.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtdpqmobeb.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gtuqjfnmad.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtvgxxvdak.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sufxvd.cn/gtkigdoyze.html

[R59] 发 POST JSON
来源：http://hz.vqdsnc.cn/gtkcxpfmxr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtdglexhxw.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgfzy.top/gtrvegtnay.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangkeji.top/gtarhwdlxi.html

[R61] 磁盘占用
来源：http://hz.nanxinkj.top/gtgtlhexpw.html

df -h;  du -sh *
来源：http://hz.fzhhl.top/gtgmtakyxz.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtmfmfuvlj.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtddishlxf.html

[R63] 内存与进程
来源：http://hz.shuidangran.top/gtgiisguql.html

free -h;  ps aux | grep nginx
来源：http://hz.jinghuilouyu.cn/gtftfilazk.html

[R64] 结束进程
来源：http://hz.xylfe.cn/gtehpetise.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenjidiqi.icu/gtbaarmtmj.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gtvbnludkz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.9152youxi.cn/gtpccqwpgw.html

[R66] 定时任务
来源：http://hz.hnqzz.top/gtmhbkrcrv.html

crontab -e;  crontab -l
来源：http://hz.hnqzz.top/gtptybskno.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtxfdbtriy.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtxruyuruh.html

[R68] 计算文件校验值
来源：http://hz.jlsjyb.cn/gtbmxiaxtk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yvedp.cn/gtmbfhvbuv.html

[R69] 生成随机密码
来源：http://hz.jinyuanbaomall.cn/gtlxgeceyc.html

head -c 16 /dev/urandom | base64
来源：http://hz.daxiang520.top/gtdhkutehb.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gtsdharpbe.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangtech.top/gtsdnsfsfm.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtqasxvjpa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtidelrbaj.html

[R72] 等待端口就绪
来源：http://hz.zhengqikj.top/gtlnsjchie.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gotoacloud.top/gtfwrrehvp.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gtdvvxndtb.html

split -l 1000 big.log part_
来源：http://hz.cqqwz.cn/gtvllroury.html

[R74] 批量重命名
来源：http://hz.wangshuangyany.cn/gtnwdfpyiy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gttaqscpao.html

[R75] 导出环境变量
来源：http://hz.sufxvd.cn/gtyqdqpone.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtsoivpdsk.html

[R76] 使用临时文件
来源：http://hz.tianlin.xyz/gtkwanqmyx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtzwtcxlxx.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtzhloxfuv.html

read -rp "请输入: " ans
来源：http://hz.yuanzhike.top/gtbwuvunbh.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtczxuzfsm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtdzhhphuo.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtaqhanwrc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ybcxt.top/gtbivmbhdn.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtawigdufu.html

time ./run.sh
来源：http://hz.yj20258888.top/gtdoqbomwr.html

================================================================================
来源：http://hz.andypj.xyz/gtmitnrbcf.html

S. C / C++ 专题
来源：http://hz.chenjidiqi.icu/gttkquqmfr.html

================================================================================
来源：http://hz.yuxming.cn/gtfmhdoibi.html

[S01] C：Hello World
来源：http://hz.daria6918.cn/gthzxbwuhk.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtqsppieen.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxuanxn.top/gtormzqjkx.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtbckkbhep.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydjk.org.cn/gtkdurtvil.html

[S03] C：读入整数
来源：http://hz.sysykeji.top/gtuqlxxygr.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtsyhoeqkn.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtqscajkcm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hfpthk.cn/gtwqumerau.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtvxoxpbfc.html

strlen(s)
来源：http://hz.gogol.net.cn/gtasjoygzz.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtnihrxybo.html

strcmp(a, b) == 0
来源：http://hz.yangfankeji.com/gthnkhlhbm.html

[S07] C：数组遍历求和
来源：http://hz.zhaomingkeji.xyz/gtmnonzgdk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtyyfderza.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtvdxrpsor.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tanke756.top/gtadwiqavf.html

[S09] C：结构体定义与初始化
来源：http://hz.hfpthk.cn/gtmpndkycv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangdashe.top/gtdpiwrvjl.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtcnmtnkik.html

int *p = &a;  *p = 5;
来源：http://hz.tian-w.cn/gtczhccrag.html

[S11] C：逐行读文件
来源：http://hz.sxryk.cn/gtplpldsqi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigfzy.top/gtwtivnzkd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtnicyacth.html

fclose(f);
来源：http://hz.yanxiufei.cn/gtwmwvozwr.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gtmhlcfheu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtfqibdwoc.html

[S13] C：宏定义
来源：http://hz.daxiang520.top/gtjwwfxrne.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cashguo.top/gtejovybxm.html

[S14] C：枚举
来源：http://hz.kuanghao11.cn/gtmxreqpdt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gtcgmrqtaq.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtqzeryxad.html

(double) a / b
来源：http://hz.zhaomingkeji.xyz/gtvjmtnwaa.html

[S16] C：位操作置位
来源：http://hz.xuanzx.com/gtxkqtqnut.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtflxjknme.html

[S17] C：安全拼接字符串
来源：http://hz.xinyue.icu/gtqwklccia.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gthckgwgrd.html

[S18] C：命令行参数
来源：http://hz.quarkkingdee.top/gtlbfpedor.html

int main(int argc, char **argv)
来源：http://hz.gzhubu.top/gtbwckkkuc.html

[S19] C：快速排序
来源：http://hz.jianghu66.top/gtrkalqbdf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtkqmrfrla.html

[S20] C：二分查找
来源：http://hz.pycfn.com/gtfisstcnm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtdaegzznm.html

[S21] C：字符类别判断
来源：http://hz.yongpay.top/gtloiqmpfp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.andypj.xyz/gtqmcsccuq.html

[S22] C：字符串转数字
来源：http://hz.havefunace.top/gtmnoudstl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zycfv.cn/gtogxctjdw.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtxuguwztx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gthzgswmqp.html

[S24] C：获取本地时间
来源：http://hz.ehwqpu.com/gtsrdbydvm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gtmvohjzts.html

[S25] C：内存拷贝
来源：http://hz.kuanghao11.cn/gtymhgjtca.html

memcpy(dst, src, n);
来源：http://hz.shuidangran.top/gtwzllzrlx.html

[S26] C：内存清零
来源：http://hz.jinyuanbaomall.cn/gtvlbzvxmi.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtikyqbquq.html

[S27] C：定义常量
来源：http://hz.tian-w.cn/gtveiaeann.html

const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtozanaktv.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtcyqjyxdo.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtepolgcts.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gtaaknlbra.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fengsongda.top/gtbvpbovmb.html

[S30] C：头文件保护
来源：http://hz.nanxinkj.top/gtimqbdiva.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtrlyugkiz.html

#define X_H
来源：http://hz.tianlin.xyz/gtqomublom.html

#endif
来源：http://hz.daxiang520.top/gtacezqxpx.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gttwyouqjj.html


<!-- 参考信息 -->