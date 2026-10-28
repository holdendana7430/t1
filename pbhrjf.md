代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.9152youxi.cn/gtonwjqjsz.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtznkluhpm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtqdjoknyj.html

[Q70] 更新统计信息
来源：http://hz.hfpthk.cn/gtdeftpcvb.html

ANALYZE TABLE users;
来源：http://hz.jyoumei.cn/gtwdpnqerb.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtowhichlh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gtmlbcwykd.html

[Q72] 查看索引
来源：http://hz.wangdashe.top/gtgvcctccw.html

SHOW INDEX FROM users;
来源：http://hz.yanxiufei.cn/gtstqqyhiu.html

[Q73] 查看表状态
来源：http://hz.ydzc1.top/gtyiiayggf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigufen.top/gtuhzvyrub.html

[Q74] 强制使用索引
来源：http://hz.xinyue.icu/gtqcupzgyp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtqyptaqut.html

[Q75] 日期格式化
来源：http://hz.kuanghao11.cn/gtxsxwsngf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cucudq.cn/gtihmrxeeu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xingfuxueyuan.xyz/gtcoheieki.html

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gthwgsaikg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.birdmap.top/gtrzdheaii.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtkawukukk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dashuyun.cn/gtutvrgnha.html

[Q78] 当前时间
来源：http://hz.shangyingyoupin.top/gtmlqidmny.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtktxjnxel.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtuqvdpiuc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gogol.net.cn/gtxxrdadyw.html

[Q80] 字符串截取
来源：http://hz.dashuyun.cn/gtspqqilky.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jianghu66.top/gteuaswerf.html

[Q81] 字符串替换
来源：http://hz.zdqjudy.top/gtwnpbxwzt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.iojbl.cn/gtubgynzwb.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtqqlhdigx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gtxeigzclw.html

[Q83] 大小写转换
来源：http://hz.zhixingplan.top/gtgdvtizcs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aizwys.cn/gtyrmkoqso.html

[Q84] 去除首尾空格
来源：http://hz.xinyue.icu/gthobwyexy.html

SELECT TRIM(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtzceoqppi.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtquaqvvsk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.iojbl.cn/gtnzulvjun.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtkiyuqnue.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtqubjhamm.html

[Q87] JSON 字段做条件
来源：http://hz.yueranfly.top/gtrolhldcl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zdqjudy.top/gtgerrbgwf.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenzaomai.com/gtndldaygq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtcduglsvu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hongshengwenyu.top/gtknacdryn.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtvoaoizhh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.vqdsnc.cn/gtlaktsdvi.html

[Q90] 生成序号列
来源：http://hz.jinghuilouyu.cn/gtcixjqiyv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yangfankeji.com/gtueorpzml.html

================================================================================
来源：http://hz.yongpay.top/gthboexdqs.html

R. Bash 专题
来源：http://hz.gotoacloud.top/gtxdwssejs.html

================================================================================
来源：http://hz.xinyue.icu/gtjirbqszt.html

[R01] shebang 与严格模式
来源：http://hz.jiagoushi.top/gtuokgoadl.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gtrvueusxk.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtpsmwvgjx.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtxxnjsgdb.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtkhdttjom.html

[R03] 只读变量
来源：http://hz.gotoacloud.top/gtzvecsomt.html

readonly PI=3.14
来源：http://hz.cashguo.top/gthkdcbpmz.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gtlnobclmo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigfzy.top/gtwytxqcif.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtiwzsfzwp.html

name="${1:-default}"
来源：http://hz.zycfv.cn/gttbpwjobc.html

[R06] 判断命令是否存在
来源：http://hz.yj202588.top/gtaynihvtj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtjioqhfqv.html

[R07] if 判断文件
来源：http://hz.jiagoushi.top/gtykytfkjd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangdashe.top/gtkohfumjh.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gttdxyvcvk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dianchejie.cn/gtxdijdhbp.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtdginocxk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ywan-chungtsiang.top/gtvvulurwn.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtawnxfkma.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258888.top/gthuajuljb.html

[R11] case 多分支
来源：http://hz.fengsongda.top/gtlcgemlil.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtkwxqkqbe.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtbzcdpshm.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangtech.top/gtsxocrhag.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtweuvbtoq.html

esac
来源：http://hz.zhongyouzk.top/gtwynojags.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtuqwymrnj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtbfqwizwu.html

[R13] for 计数循环
来源：http://hz.9152youxi.cn/gtzulnzjpl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hammf.cn/gtjprzcubj.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gtnitopfmj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fengsongda.top/gtpkkxncsj.html

[R15] while 逐行读文件
来源：http://hz.52xcode.cn/gtanymsdlp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nwbrower.top/gtwtceoeyi.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtkjlpsaoh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtkappstgq.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtvhafaruh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xingfuxueyuan.xyz/gtzsckxlod.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gteqkselwh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ywan-chungtsiang.top/gtsoomadia.html

[R19] 数组长度
来源：http://hz.aibaodan.cn/gtiluqvkzr.html

echo "${#arr[@]}"
来源：http://hz.hysaishi.cn/gttuuypzxi.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gthhtvrzkh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gttxxjceqr.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtsrwivedm.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtziebpsot.html

[R22] 截取子串
来源：http://hz.zdqjudy.top/gtqcrbeoem.html

echo "${s:0:5}"
来源：http://hz.9152youxi.cn/gtbxxdjljo.html

[R23] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gthspgarzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.9152youxi.cn/gtxjlcdixm.html

[R24] 大小写转换
来源：http://hz.svipenyu.cn/gtxxbmmsfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gtetkrntsa.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinghuilouyu.cn/gtcyqgetfz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtqhkqeqxv.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gthfemdxla.html

now=$(date +%F); echo "$now"
来源：http://hz.jyoumei.cn/gtgeqxgoqk.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtiwzwaumg.html

echo $((1 + 2 * 3))
来源：http://hz.vqdsnc.cn/gtrhdyhhrd.html

[R28] 浮点运算
来源：http://hz.xziqi.cn/gtovvhwhop.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenjidiqi.icu/gtctqywysh.html

[R29] 定义函数
来源：http://hz.chenjidiqi.icu/gtitsxvzrt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigfzy.top/gtcighvmkx.html

[R30] 函数返回状态码
来源：http://hz.haohaochexian.top/gtqglnvopl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydzc1.top/gtlupztapz.html

[R31] 局部变量
来源：http://hz.9152youxi.cn/gtflmrqvfu.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gttcwrsfbw.html

[R32] 参数个数校验
来源：http://hz.daxiang520.top/gtgikmfbef.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtbtgjkiwx.html

[R33] 捕获错误并提示行号
来源：http://hz.ybcxt.top/gtlwhmcuph.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtnwljcryi.html

[R34] 退出时清理
来源：http://hz.xuanzx.com/gtqhuaeigm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtsjvocfvo.html

[R35] 后台执行并等待
来源：http://hz.zhoulong.xyz/gtdepasnpp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gtcqapdvfx.html

[R36] 并发执行多个任务
来源：http://hz.zhongyouzk.top/gtffovdylu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuetiantiany.cn/gticcmaxag.html

[R37] 把输出赋给变量
来源：http://hz.tian-w.cn/gtjwqpczoy.html

files=$(ls -1)
来源：http://hz.feifeiyinyue.top/gtxiymqbae.html

[R38] 管道串联
来源：http://hz.316326.xyz/gtxnehjxvs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shzxlz.cn/gtlcdvhusn.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtsgcxnymm.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtzdqyvvjs.html

[R40] 追加写日志
来源：http://hz.cashguo.top/gtohgucqxx.html

echo "log" >> out.log
来源：http://hz.jinqigufen.top/gtkbkjdopc.html

[R41] 丢弃输出
来源：http://hz.snrcjt.cn/gthbgeikva.html

cmd >/dev/null 2>&1
来源：http://hz.redwolf501.top/gtacseuwrp.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gttaivyqcn.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtgbomxbix.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gthtjpjaus.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gtlsppxcnj.html

[R44] 按修改时间查找
来源：http://hz.guannengcc.top/gticraysba.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtbgdapxru.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gthsnbiegh.html

find . -name "*.tmp" -delete
来源：http://hz.yangfankeji.com/gtdxnhjwtj.html

[R46] 递归替换文件内容
来源：http://hz.hywenlv.cn/gtrhfiywca.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydzc1.top/gtkabthvxa.html

[R47] sed 单行替换
来源：http://hz.aibaodan.cn/gtlpjfrkut.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gttwedxumr.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtartdhfnf.html

awk '{print $1, $3}' a.txt
来源：http://hz.hysaishi.cn/gtlzfqdgdb.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtjyvyqyce.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenzaomai.com/gtleyqxyzl.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtuiwbdbxn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuxming.cn/gtjigmtzcc.html

[R51] 排序去重取前几
来源：http://hz.zycfv.cn/gtopxhsfdh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhoulong.xyz/gtkkckyvnq.html

[R52] 统计行数
来源：http://hz.andypj.xyz/gtdswotczx.html

wc -l a.txt
来源：http://hz.nanxuanxn.top/gtdflcodyx.html

[R53] 查看文件头与实时尾
来源：http://hz.gzhubu.top/gtkfhiljuk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydzc1.top/gtgbwuwjyv.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangtech.top/gtsfyynwiz.html

diff a.txt b.txt
来源：http://hz.tian-w.cn/gtpujsisgb.html

[R55] 压缩与解压
来源：http://hz.andypj.xyz/gtthahrmnm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtujwolcxx.html

[R56] 远程拷贝
来源：http://hz.gotoacloud.top/gtoxvbxagm.html

scp file user@host:/path/
来源：http://hz.guannengcc.top/gtuqlljbpv.html

[R57] 远程执行命令
来源：http://hz.ehwqpu.com/gtvxfpfjpc.html

ssh user@host 'uptime'
来源：http://hz.quarkkingdee.top/gtvgvvtxpy.html

[R58] 下载文件
来源：http://hz.cucudq.cn/gtqwnofudm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.haohaochexian.top/gtvgdlhlyw.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtyfzocefq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenlongwang.top/gtiwmrqsnl.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtnreknpdq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sweek.top/gtgdzvycbo.html

[R61] 磁盘占用
来源：http://hz.ivvv.top/gtibwgbauf.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gthdsisaig.html

[R62] 找最占空间的文件
来源：http://hz.shzxlz.cn/gtksbovjby.html

du -ah . | sort -rh | head -10
来源：http://hz.zhengqikj.top/gthiktmiuc.html

[R63] 内存与进程
来源：http://hz.gzhubu.top/gtqpmxuwlt.html

free -h;  ps aux | grep nginx
来源：http://hz.yuxming.cn/gtafuuktzc.html

[R64] 结束进程
来源：http://hz.yuanzhike.top/gtbzvcbnxi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtbcizwpqe.html

[R65] 查看端口占用
来源：http://hz.feifeiyinyue.top/gtfgmgxapd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtejkbbphh.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtbhokyyml.html

crontab -e;  crontab -l
来源：http://hz.chenjidiqi.icu/gtnetacqda.html

[R67] 生成随机十六进制串
来源：http://hz.birdmap.top/gtqcrxqgei.html

openssl rand -hex 16
来源：http://hz.chenlongwang.top/gtwmpaaeuc.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtngvvjeek.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gtfwzrmdba.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtnjmywvln.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtlwavchrh.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gttqrihulv.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gtlzwdxweh.html

[R71] 日期格式化
来源：http://hz.sufxvd.cn/gtnduubrtp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.316326.xyz/gtjknqzrvp.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtimgyqkwb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shzxlz.cn/gtpzjbtmdv.html

[R73] 分割大日志
来源：http://hz.jiagoushi.top/gtgwecgfrk.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtveiimmrx.html

[R74] 批量重命名
来源：http://hz.hnqzz.top/gtalpnhmxh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sufxvd.cn/gtdidccsce.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtkpkoarmu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gttxogjzxq.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtgkzmdqzy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtsmkahxtj.html

[R77] 读取用户输入
来源：http://hz.sysykeji.top/gtvygaaxww.html

read -rp "请输入: " ans
来源：http://hz.zhixingplan.top/gtqqyipmcz.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gtbgzzpjnq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cashguo.top/gtgmkzlcpj.html

[R79] 解析命令行选项
来源：http://hz.xylfe.cn/gtjhynjrxy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.haohaochexian.top/gtgpxibajp.html

[R80] 查看脚本执行耗时
来源：http://hz.vqdsnc.cn/gtwcozxmyt.html

time ./run.sh
来源：http://hz.yonumen.top/gtanlxsvwr.html

================================================================================
来源：http://hz.ivvv.top/gttafspdcz.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtuwchwzbo.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnaqkohti.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gtgrtqkxra.html

#include <stdio.h>
来源：http://hz.hammf.cn/gtnkbfwelh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtknrhtqsb.html

[S02] C：变量与格式化输出
来源：http://hz.hnqzz.top/gttphcbzbr.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtbkgjxura.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gttiltywsc.html

int x; scanf("%d", &x);
来源：http://hz.jinyuanbaomall.cn/gtxwgkspyy.html

[S04] C：字符串复制
来源：http://hz.sysykeji.top/gtbeypdwpk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgfzy.top/gtqttvssgt.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gtlkhyxnke.html

strlen(s)
来源：http://hz.yj202588.top/gtakhpufme.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gtrqzeqlyh.html

strcmp(a, b) == 0
来源：http://hz.jiagoushi.top/gtiviocwnp.html

[S07] C：数组遍历求和
来源：http://hz.ehwqpu.com/gtircduixz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xingfuxueyuan.xyz/gtjnxfqpfu.html

[S08] C：动态内存分配与释放
来源：http://hz.yuanzhike.top/gtejzyasoa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtkymghvch.html

[S09] C：结构体定义与初始化
来源：http://hz.smart0.xyz/gttdyjekcr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.316326.xyz/gtklmehsft.html

[S10] C：指针与解引用
来源：http://hz.jianghu66.top/gttdixvmaw.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gttatxwrio.html

[S11] C：逐行读文件
来源：http://hz.wangdashe.top/gtbascndmg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.haohaochexian.top/gtdsolxuzf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtxomdnxei.html

fclose(f);
来源：http://hz.cheryme.top/gtmxddnoxt.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtjnojrlur.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtqemelpju.html

[S13] C：宏定义
来源：http://hz.wangshuangyany.cn/gtgfzvbolv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtzdcsrpjg.html

[S14] C：枚举
来源：http://hz.sysykeji.top/gtedruqyub.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuetiantiany.cn/gtydeavfnf.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtjnjegjbl.html

(double) a / b
来源：http://hz.nanxuanxn.top/gtfsxkndbt.html

[S16] C：位操作置位
来源：http://hz.xuanzx.com/gtafufwtof.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtgkgdhesi.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtrcjbjchc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jlsjyb.cn/gtztvrqfpe.html

[S18] C：命令行参数
来源：http://hz.jqgufenzy.top/gtgurvvmbz.html

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gtzssdkbnw.html

[S19] C：快速排序
来源：http://hz.cdnleiting.top/gtowzmroue.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtcnwqfxpd.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtjfffpwfe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtiebqtgup.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtjcszjoun.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.9152youxi.cn/gtkgfzqgfd.html

[S22] C：字符串转数字
来源：http://hz.zhaomingkeji.xyz/gtrpihftys.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gtyvtggbmd.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtyuxkwylm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuxming.cn/gtleftwzfr.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtetghfohc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.smart0.xyz/gttoxsoygw.html

[S25] C：内存拷贝
来源：http://hz.iojbl.cn/gtrsevugdo.html

memcpy(dst, src, n);
来源：http://hz.pengpengdd.cyou/gtloxgpkav.html

[S26] C：内存清零
来源：http://hz.yanxiufei.cn/gtxccyoqgy.html

memset(a, 0, sizeof a);
来源：http://hz.nanxuanxn.top/gtrzqenfog.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtyyklvkvw.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtbvtlcnfm.html

[S28] C：静态变量
来源：http://hz.shangyingyoupin.top/gtyswkxtmi.html

static int counter = 0;
来源：http://hz.aibaodan.cn/gtcugcopkm.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtqsybcjpa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtaawsfkne.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtoznnygqd.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gtwvjchbjl.html

#define X_H
来源：http://hz.yonumen.top/gtiiorrsqk.html

#endif
来源：http://hz.nanxinkj.top/gtnolnjpei.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtdobfnabg.html

#include <iostream>
来源：http://hz.pengpengdd.cyou/gttzorrqmr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gtsnqcsime.html

[S32] C++：字符串
来源：http://hz.cheryme.top/gtewsfiqan.html

std::string s = "hi";  s += "!";
来源：http://hz.dianchejie.cn/gteujaizlf.html

[S33] C++：vector 增删
来源：http://hz.wangshuangyany.cn/gtlfyemvgl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xinyue.icu/gtdawfklgk.html

[S34] C++：遍历 vector
来源：http://hz.havefunace.top/gtyhxkhcbq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.iojbl.cn/gtvnwlarzj.html

[S35] C++：map
来源：http://hz.zhongyouzk.top/gtqwhmjiyo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtwytfivhd.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtwdimpbpw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtohlxujhz.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gtjjywucix.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtjldjwzkg.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtxwoqglpn.html

std::sort(v.begin(), v.end());
来源：http://hz.shangyingyoupin.top/gtfjoafshq.html


<!-- 参考信息 -->